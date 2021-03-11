cmake_minimum_required(VERSION 2.8)
project(camera_calibration)
find_package(OpenCV REQUIRED)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(${OpenCV_INCLUDE_DIRS})

#OpenCV C++ book
add_executable(camera_calibration main.cpp)


target_link_libraries(camera_calibration ${OpenCV_LIBS})
