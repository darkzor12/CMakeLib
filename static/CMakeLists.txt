cmake_minimum_required(VERSION 3.20)

project(static_lib)

add_library(static_lib STATIC static_lib.cpp)

target_include_directories(static_lib
    PUBLIC 
        ${PROJECT_SOURCE_DIR}/static
)