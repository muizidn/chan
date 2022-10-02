cmake_minimum_required(VERSION 3.24.2)
project(chan VERSION 0.0.4 DESCRIPTION "Pure C implementation of Go channels.")
add_library(chan SHARED
    src/chan.c
    src/queue.c
)

set_target_properties(chan PROPERTIES PUBLIC_HEADER 
    src/chan.h
)
target_include_directories(chan PRIVATE src)

add_subdirectory(examples)