
cmake_minimum_required(VERSION 3.22.2)
project(people_detect VERSION 1.0)

add_executable(people ${PROJECT_NAME}.cpp)
find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(people ${OpenCV_LIBS})

set(CMAKE_SYSTEM_NAME Windows)
set(CMAKE_SYSTEM_PROCESSOR intel)

#set(CMAKE_CXX_FLAGS "-std=c++11")
set(CMAKE_CXX_COMPILER "C:/MinGW/bin/g++")
