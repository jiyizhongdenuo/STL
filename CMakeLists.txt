cmake_minimum_required(VERSION 3.20)

project(Hello)

add_subdirectory(src)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
include_directories(include)
add_compile_options(-Wall)
set(CMAKE_BUILD_TYPE Debug)
# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++20")

add_executable(main main.cpp src/swap.cpp)
