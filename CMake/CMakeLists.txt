cmake_minimum_required()    # Minimum required version for project:    cmake_minimum_required(VERSION 3.1)
project()                   # Name of project + language:              project(binary_tree C)
set()                       # What C Make standard. Just use:          set(CMAKE_C_STANDARD 11)

add_executable()            # Name of executable and file path:         add_executable(binary_tree binary_tree.c)

add_library()               # Name of header and header source name:   add_library(binary_tree_lib binary_tree.h)
                            # Only if the header gets something from another header file or
                            # the c file gets something from another c file

target_link_libraries()     # Name of executable and name of library:  target_link_libraries(binary_tree binary_tree_lib)

add_subdirectory()          # Path to subdirectory                  :  add_subdirectory(Projects/binary_search/binary_tree)