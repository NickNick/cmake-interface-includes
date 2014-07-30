cmake_minimum_required(VERSION 2.8.12)

add_library(foo foo/foo.cpp)
target_include_directories(foo INTERFACE foo)

add_library(bar bar/bar.cpp)
target_link_libraries(bar foo)
