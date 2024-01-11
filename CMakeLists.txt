cmake_minimum_required(VERSION 3.26)
project(UnityExample)

set(CMAKE_C_STANDARD 11)

include_directories(include)
include_directories(library/Unity/include) 

add_subdirectory(source)
add_subdirectory(test)

