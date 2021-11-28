cmake_minimum_required(VERSION 3.5)
project(FRay VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 20)

#execute_process(COMMAND git submodule update --init --recursive
#    WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR})

#find_package(Boost 1.68 REQUIRED)
#include_directories(
#    ${Boost_INCLUDE_DIRS}
#    extern/NumCpp/include
#    )

#file(GLOB FRAY_TARGETS
#    FRay.cpp
#    World/*.cpp
#    )
#add_library(FRay STATIC ${FRAY_TARGETS})

add_executable(testFRay testFRay.cpp)
#target_link_libraries(testFRay PRIVATE FRay)
