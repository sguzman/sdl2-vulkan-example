cmake_minimum_required(VERSION 3.16)
project(vulkan-example C++)
set (CMAKE_CXX_STANDARD 11)

set(CMAKE_VERBOSE_MAKEFILE "TRUE")
set(CMAKE_CXX_COMPILER "/usr/bin/clang")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra")

set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -g")
set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} -O3")

add_executable(vulkan-example main.cpp vulkan_extern.cpp  vulkan_extern.h  vulkan_function.cpp  vulkan_function.h)
