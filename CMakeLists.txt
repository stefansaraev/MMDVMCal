cmake_minimum_required(VERSION 2.6)

set(APP_NAME "MMDVMCal")
project(${APP_NAME})

file(GLOB SOURCES "*.cpp")
file(GLOB HEADERS "*.h")

SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Os -Wall -std=c++0x $ENV{CXXFLAGS}")

add_executable(${APP_NAME} ${SOURCES} ${HEADERS})
