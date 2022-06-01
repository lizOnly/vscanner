cmake_minimum_required(VERSION 3.22)

project(scanner)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

if(NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()

find_package(gproshan REQUIRED)

include_directories(SYSTEM ${gproshan_INCLUDE_DIR})

add_executable(scanner src/main.cpp)
target_link_libraries(scanner gproshan) 