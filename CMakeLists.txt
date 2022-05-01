cmake_minimum_required(VERSION 3.10)

# set the project name
project(Tutorial)

file(GLOB_RECURSE SOURCES src/*.cpp)

# add the executable
add_executable(Tutorial ${SOURCES})

target_include_directories(Tutorial PUBLIC include)

set(GLFW_BUILD_DOCS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_TESTS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)

add_subdirectory(ext/glfw)
target_link_libraries(Tutorial glfw)

add_subdirectory(ext/glad)
target_link_libraries(Tutorial glad)

find_package(OpenGL REQUIRED)
target_link_libraries(Tutorial OpenGL::GL)