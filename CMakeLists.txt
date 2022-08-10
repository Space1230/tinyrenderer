cmake_minimum_required(VERSION 3.23)
project(TinyRenderer)

set(PN ${PROJECT_NAME})
set(PD ${PROJECT_SOURCE_DIR})

include_directories(${PD})

file(GLOB_RECURSE Files ${PD} *.cpp)

add_executable(${PN} main.cpp tgaimage.cpp)
