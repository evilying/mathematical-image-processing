cmake_minimum_required(VERSION 2.8)

set(CMAKE_CXX_FLAGS "-std=c++0x ${CMAKE_CXX_FLAGS}")

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(simple_canny_cli main.cpp)
target_link_libraries(simple_canny_cli ${OpenCV_LIBRARIES})
