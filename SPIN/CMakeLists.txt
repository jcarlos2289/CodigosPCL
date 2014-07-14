cmake_minimum_required(VERSION 2.6 FATAL_ERROR)

project(descriptor_spin)

find_package(PCL 1.5 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (spin spin.cpp)
target_link_libraries (spin ${PCL_LIBRARIES})
