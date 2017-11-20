cmake_minimum_required(VERSION 3.5)
project(Reconstruction3D)

find_package (OpenCV REQUIRED)
set(CMAKE_CXX_STANDARD 14)

file(GLOB SRC src/*.cpp )
add_executable(Analyse ${SRC})
target_link_libraries (Analyse ${OpenCV_LIBS})