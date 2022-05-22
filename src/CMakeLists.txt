cmake_minimum_required(VERSION 3.20)

project(hello-world LANGUAGES CXX)

add_executable(hello-world main.cpp)

find_package(Boost)

set_target_properties(hello-world PROPERTIES
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED ON
    )

add_executable(hello-world-v01 main.cpp)

set_target_properties(hello-world-v01 PROPERTIES
      CXX_STANDARD 17
      CXX_STANDARD_REQUIRED ON
      )

#set(CMAKE_CXX_STANDARD 11)
#set(CMAKE_CXX_STANDARD_REQUIRED ON)

