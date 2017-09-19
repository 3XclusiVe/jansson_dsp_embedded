
cmake_minimum_required(VERSION 3.0)
project(ArduinoJson)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

add_definitions(-include ntsid.h)

file(GLOB_RECURSE SRCS *.cpp *.c)
file(GLOB_RECURSE HDRS *.h *.hpp)

ADD_EXECUTABLE(src  ${SRCS} ${HDRS} )
