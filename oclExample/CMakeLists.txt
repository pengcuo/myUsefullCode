cmake_minimum_required(VERSION 2.8)
#include(hpcc-common)
#include_directories("/home/android-toolchain-armv7/include")
#link_directories("/home/android-toolchain-armv7/lib/OpenCL/qualcomm")


set(CMAKE_MODULE_PATH /home/pengcuo/cmake)
include(toolchain)
project(OpenCLAdd)


add_executable(ocl_example ocl_example.cpp)
target_link_libraries(ocl_example OpenCL)
