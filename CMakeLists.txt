set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(UniversityDB)
cmake_minimum_required(VERSION 2.8)
aux_source_directory(. SRC_LIST)
include_directories(includes)
add_definitions(-Wall -Wextra -Wpedantic -Werror)
add_executable(${PROJECT_NAME} ${SRC_LIST})
