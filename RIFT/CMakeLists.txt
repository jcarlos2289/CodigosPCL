cmake_minimum_required(VERSION 2.6 FATAL_ERROR)

project(descriptor_rift)

find_package(PCL 1.5 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (rift rift.cpp)
target_link_libraries (rift ${PCL_LIBRARIES})
