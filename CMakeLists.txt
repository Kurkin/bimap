cmake_minimum_required(VERSION 2.8)

project(bimap)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Wall -Wextra -pedantic -fsanitize=address")

add_executable(bimap_test 
            gtest/gtest-all.cc
            gtest/gtest.h
            gtest/gtest_main.cc
            src/bimap.hpp
            src/test.cpp)
