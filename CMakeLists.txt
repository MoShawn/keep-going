cmake_minimum_required(VERSION 3.10)
project(keep_going LANGUAGES C)
# 头文件包含
include_directories(${CMAKE_SOURCE_DIR}/array)
# 包含子目录
add_subdirectory(array)
add_executable(keep_going main.c)
target_link_libraries(keep_going array)