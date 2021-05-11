cmake_minimum_required(VERSION 3.17)
project(niaisage_disco)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory("lib/libdiscobot")

add_executable(disco main.cpp)
add_dependencies(disco libdisco)

target_include_directories(disco PRIVATE "lib/libdiscobot/include")
