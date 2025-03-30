cmake_minimum_required(VERSION 3.12)
set(CMAKE_CXX_STANDARD 17)

message("log****VCPKG_ROOT  PATH:$ENV{VCPKG_ROOT}")
project(MYGAMES101)
# set(CMAKE_INSTALL_PREFIX ${CMAKE_SOURCE_DIR})

set(WITH_GTK 0)

add_subdirectory(00)
add_subdirectory(01)
add_subdirectory(02)
add_subdirectory(03)

install(TARGETS 00 01 02 03 DESTINATION output)