cmake_minimum_required(VERSION 3.8)
set(CMAKE_CXX_STANDARD 11)
project(hw3)

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

set(SOURCE_FILES main.cpp)
add_executable(hw3 ${SOURCE_FILES})
target_link_libraries (hw3 ${OpenCV_LIBS})