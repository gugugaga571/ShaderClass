cmake_minimum_required(VERSION 3.10)
project(ShaderClass)

set(CMAKE_CXX_STANDARD 17)

include_directories("D:/glfw-3.5.1/glfw-3.5.1/include")
include_directories("D:/glad/include")

link_directories("D:/glfw-3.5.1/glfw-3.5.1/build/src/Release")

add_executable(ShaderClass main.cpp glad.c Shader.cpp)

target_link_libraries(ShaderClass glfw3.lib opengl32.lib)