cmake_minimum_required(VERSION 2.8)

set(curr_dir ${CMAKE_CURRENT_SOURCE_DIR})
set(hello_dir ${curr_dir}/hello)
set(world_dir ${curr_dir}/world)

project(helloworld)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

# Add header file include directories
include_directories(
    ${hello_dir}/include
    ${world_dir}/include
)

# Add block directories
add_subdirectory(hello)
add_subdirectory(world)
# Target
add_executable(helloworld main.cpp)
target_link_libraries(helloworld hello world)