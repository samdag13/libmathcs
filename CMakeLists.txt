# CMake 3.30 is fairly new and not available on all systems. The
# current build environment provides CMake 3.28, so requiring 3.30
# prevents the project from building. Lower the requirement to a more
# common version to allow building with the provided tools.
cmake_minimum_required(VERSION 3.10)
project(untitled)

set(CMAKE_CXX_STANDARD 20)

add_library(untitled SHARED library.cpp)
