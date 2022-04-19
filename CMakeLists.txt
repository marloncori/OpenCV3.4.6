
cmake_minimum_required(VERSION 3.22.2) # change this according to your CMake version
project(<write here the file name with no .cpp> VERSION 1.0)

add_executable(<repeat here the Cpp file name without .cpp> ${PROJECT_NAME}.cpp)
find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(<repeat here the Cpp file name without .cpp> ${OpenCV_LIBS})

set(CMAKE_SYSTEM_NAME Windows) # change this according to your machine
set(CMAKE_SYSTEM_PROCESSOR intel) # change this according to your machine

#set(CMAKE_CXX_FLAGS "-std=c++11") # change this according to your C++ version
set(CMAKE_CXX_COMPILER "C:/MinGW/bin/g++") # change this according to your machine
