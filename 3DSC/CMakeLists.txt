cmake_minimum_required(VERSION 2.6 FATAL_ERROR)

project(descriptor_3dsc)

find_package(PCL 1.5 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (3dsc 3dsc.cpp)
target_link_libraries (3dsc ${PCL_LIBRARIES})
