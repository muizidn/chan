cmake_minimum_required(VERSION 3.24.2)
project(unbuffered)
add_executable(unbuffered 
    unbuffered.c
)

target_link_libraries(unbuffered chan)