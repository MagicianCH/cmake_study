cmake_minimum_required(VERSION 3.0)
project(cmake_study)

set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)

include_directories(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)
set(HELLO_LIB hello world)

message(STATUS ${HELLO_LIB})
add_subdirectory(src)
