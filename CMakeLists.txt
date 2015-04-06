cmake_minimum_required(VERSION 2.8)

set(PROJECT_NAME teensy-template)
project(${PROJECT_NAME})

teensy_add_executable(${PROJECT_NAME} source/main.cpp)
