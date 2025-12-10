# Création de la librairie
add_library(lib
    lib/calculator.c
)

# Création de l'exécutable
add_executable(calculator
    main.c
)

# Lier l'exécutable avec la librairie
target_link_libraries(calculator lib)

# Tests automatisés
add_test(t1 calculator add 2 3)
add_test(t2 calculator sub 3 -2)
add_test(t3 calculator mul 5 5)
add_test(t4 calculator div 1 5)
add_test(t5 calculator car 5)

