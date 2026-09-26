cmake_minimum_required(VERSION 3.10.2)
project(menu)

add_library(menu SHARED main.cpp)

find_library(log-lib log)
find_library(gles-lib GLESv3)

target_link_libraries(menu ${log-lib} ${gles-lib})
