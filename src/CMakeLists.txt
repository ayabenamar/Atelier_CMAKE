cmake_minimum_required(VERSION 3.10)
project(Atelier_CMAKE)

# ➜ Ajoutez cette ligne
include_directories(include)

add_library(lib src/lib/calculator.c)

add_executable(calculator src/main.c)

target_link_libraries(calculator lib)

# Vos tests
add_test(t1 calculator add 2 3)
add_test(t2 calculator sub 3 -2)
add_test(t3 calculator mul 5 5)
add_test(t4 calculator div 1 5)
add_test(t5 calculator car 5)
