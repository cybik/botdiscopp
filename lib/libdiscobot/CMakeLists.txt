cmake_minimum_required(VERSION 3.17)
project(libdiscobot)

set(CMAKE_CXX_STANDARD 20)

list(APPEND
    LIBDISCO_SOURCES
        src/saucer.cpp
)

include_directories(
    ${CMAKE_CURRENT_LIST_DIR}/include
)

add_library("libdisco"
    ${LIBDISCO_SOURCES}
)