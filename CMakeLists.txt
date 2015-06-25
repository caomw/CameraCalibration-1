cmake_minimum_required(VERSION 2.8)
project( cameraCalibration )

find_package( OpenCV REQUIRED )

#set(dir ${CMAKE_CURRENT_SOURCE_DIR}/build/)
#set(CMAKE_BUILD_DIRECTORY ${dir})

add_executable( cameraCalibration main.cpp )
target_link_libraries( cameraCalibration ${OpenCV_LIBS} )