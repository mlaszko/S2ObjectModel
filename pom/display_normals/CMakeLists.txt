cmake_minimum_required(VERSION 2.6 FATAL_ERROR)

project(display_normals)

find_package(PCL 1.2 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (display_normals main.cpp)
target_link_libraries (display_normals ${PCL_LIBRARIES})