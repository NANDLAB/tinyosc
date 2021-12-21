cmake_minimum_required(VERSION 3.5)

project(tinyosc LANGUAGES C)

add_library(tinyosc STATIC
  tinyosc.h
  tinyosc.c
)

target_include_directories(tinyosc PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")
target_compile_definitions(tinyosc PRIVATE TINYOSC_LIBRARY)
