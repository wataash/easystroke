cmake_minimum_required(VERSION 3.9)
project(easystroke)

set(CMAKE_VERBOSE_MAKEFILE on)

file(GLOB_RECURSE SRCS *.c *.cc *.h)

add_executable(zdummy ${SRCS})

add_custom_target(easystroke COMMAND cd ${PROJECT_SOURCE_DIR} && make)

#include_directories(
#    build/
#)

#add_definitions(-DHAVE_CONFIG_H)
