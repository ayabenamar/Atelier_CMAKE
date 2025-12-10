cmake_minimum_required(VERSION 3.10)
project(Atelier_CMAKE)

enable_testing()

# Dossier include
include_directories(${PROJECT_SOURCE_DIR}/include)

# Ajout du sous-dossier src/
add_subdirectory(src)

