cmake_minimum_required(VERSION 3.0)
project(cmake_study)

add_library(hello hello.cpp)
add_library(world world.cpp)
add_executable(main main.cpp)
target_link_libraries(main ${HELLO_LIB})
