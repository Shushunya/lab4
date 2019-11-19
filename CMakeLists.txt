cmake_minimum_required(VERSION 3.10)
project(Lab4)

add_library(lab4lib STATIC
    include/hellomake.h
    src/hellomake.c
    src/hellofunc.c
)

add_executable(liba
  src/hellomake.c
)

target_link_libraries(liba PRIVATE lab4lib)
