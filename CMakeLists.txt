# tfpa - ReXGlue Recompiled Project
#
# SDK boilerplate lives in generated/rexglue.cmake.

cmake_minimum_required(VERSION 3.25)
project(tfpa LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include(generated/rexglue.cmake)

# Sources
set(TFPA_SOURCES
    src/main.cpp
)

if(WIN32)
    add_executable(tfpa WIN32 ${TFPA_SOURCES})
else()
    add_executable(tfpa ${TFPA_SOURCES})
endif()

rexglue_setup_target(tfpa)
