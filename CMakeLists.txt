cmake_minimum_required(VERSION 3.23)
project(nes_emu)

set(CMAKE_CXX_STANDARD 20)
find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})
add_executable(nes_emu src/main.cpp )
target_link_libraries(nes_emu ${SDL2_LIBRARIES})
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
