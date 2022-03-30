cmake_minimum_required (VERSION 3.10)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/build)

set(CMAKE_EXPORT_COMPILE_COMMANDS on)

# set standards at the project level
set(CMAKE_CXX_STANDARD 17)

project(actions_test)

file(GLOB CXX_SOURCES ${PROJECT_SOURCE_DIR}/src/*.cpp)

add_executable(actions_test ${CXX_SOURCES})