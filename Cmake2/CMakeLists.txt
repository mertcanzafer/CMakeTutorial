# 1) Create code and Cmake File.
# 2) mkdir build
# 3) cd build
# 4) cmake .. # configure cmake
# 5) cmake ..build .
# 6) ./Executable

cmake_minimum_required(VERSION 3.20)

project(Cmake2 VERSION 1.0.0 LANGUAGES C CXX)

add_library(Library STATIC Starter.cpp)

add_executable(Executable main.cpp)

target_link_libraries(Executable PUBLIC Library)