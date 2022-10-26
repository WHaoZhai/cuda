cmake_minimum_required(VERSION 3.21)
project(asyncAPI CUDA)

set(CMAKE_CUDA_STANDARD 14)

include_directories(../../Common)

add_executable(asyncAPI main.cu)

set_target_properties(asyncAPI PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
