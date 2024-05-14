cmake_minimum_required(VERSION 3.28)
project(MetalTestApp)

set(CMAKE_CXX_STANDARD 23)

add_subdirectory(metal-cmake)  # Library definition

add_executable(MetalTestApp main.cpp)

target_link_libraries(MetalTestApp METAL_CPP)