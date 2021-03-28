cmake_minimum_required(VERSION 3.17)

set(PROGRAM_NAME mavlink_control)
project(${PROGRAM_NAME})

set(CMAKE_CXX_STANDARD 14)

set(MAVLINK_INCLUDES_DIR mavlink/include/mavlink/v2.0)

include_directories(${MAVLINK_INCLUDES_DIR})

add_executable(${PROGRAM_NAME} mavlink_control.cpp)
