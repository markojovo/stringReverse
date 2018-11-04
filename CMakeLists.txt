cmake_minimum_required (VERSION 2.8.11)
project (reverseString)

add_subdirectory (reverseLibrary)
include_directories (reverseLibrary)
link_directories (reverseLibrary)
add_executable (reverseString reverseString.c)

target_link_libraries(reverseString revlib)
