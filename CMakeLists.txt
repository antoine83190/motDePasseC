
cmake_minimum_required(VERSION 2.6)
		
#Déclaration du projet
project(MotdePasseenC)
set(EXECUTABLE_OUTPUT_PATH bin/${CMAKE_BUILD_TYPE})

#Génération de la liste des fichiers sources
file(
	GLOB_RECURSE
	source_files
	src/*
)

#Déclaration de l'exécutable
add_executable(
	prog
	${source_files}
)
