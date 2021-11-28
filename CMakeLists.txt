cmake_minimum_required(VERSION 3.5)
project(FRay VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 20)

execute_process(COMMAND git submodule update --init --recursive
    WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR})

find_package(Boost 1.68 REQUIRED)

#add_subdirectory(extern/NumCpp)
include_directories(${Boost_INCLUDE_DIRS} extern/NumCpp/include)
add_executable(test test.cpp)
