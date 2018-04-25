cmake_minimum_required(VERSION 3.10)
project(FINAL C)

set(CMAKE_C_STANDARD 11)

add_executable(FINAL main.c)


find_package(OpenMP)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")