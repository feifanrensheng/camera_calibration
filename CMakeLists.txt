cmake_minimum_required( VERSION 2.8 )

project( camera_calibration )

set( CMAKE_BUILD_TYPE "Release" )
set( CMAKE_CXX_FLAGS "-std=c++11 -O3" )
set( OpenCV_DIR "/usr/local/opencv-2.4.9/share/OpenCV")

find_package( OpenCV 2.4.9 REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS})

add_executable( cb cb.cpp )
target_link_libraries( cb ${OpenCV_LIBS})
