cmake_minimum_required(VERSION 3.0.0)

find_package(imgui CONFIG REQUIRED)

add_library(imnodes STATIC imnodes.cpp imnodes.h)

target_link_libraries(imnodes PRIVATE imgui::imgui)
target_include_directories(imnodes PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
