cmake_minimum_required(VERSION 2.8)

project(testQPTime)

set(CMAKE_CXX_FLAGS "-std=c++11")

link_directories("/usr/local/lib")
include_directories("/usr/local/include")

add_executable(example qp_time_test.cpp)
target_link_libraries(example libqpOASES.so)
