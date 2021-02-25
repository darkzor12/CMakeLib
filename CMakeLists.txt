cmake_minimum_required(VERSION 3.20)

project(lib)

message("Adding static subdirectory")

add_subdirectory(static)

message("Adding dynamic subdirectory")

add_subdirectory(dynamic)

add_executable(libBin main.cpp)

target_link_libraries(libBin PRIVATE static_lib)