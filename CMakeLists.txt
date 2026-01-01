cmake_minimum_required(VERSION 3.5)
project(mygame)

# Prerequisites:
# - On macOS: brew install sdl3
find_package(SDL3 REQUIRED CONFIG REQUIRED COMPONENTS SDL3-shared)

add_executable(mygame main.c)

target_link_libraries(mygame PRIVATE SDL3::SDL3)
