# Specify the minimum version for CMake

cmake_minimum_required(VERSION 2.8.10)

# Project's name

project(mnist)

link_directories(${CMAKE_SOURCE_DIR}/opennn)

include_directories(${CMAKE_SOURCE_DIR}/opennn)

add_executable(mnist main.cpp)

target_link_libraries(mnist opennn)


