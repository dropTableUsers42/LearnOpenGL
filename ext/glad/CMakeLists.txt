cmake_minimum_required(VERSION 3.10)

# set the project name
project(GLAD)

# add the library
add_library(glad src/glad.c)

target_include_directories(glad PUBLIC include)