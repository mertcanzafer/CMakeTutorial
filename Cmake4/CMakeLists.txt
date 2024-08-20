# 1) Create code and Cmake File.
# 2) mkdir build
# 3) cd build
# 4) cmake .. # configure cmake
# 5) cmake ..build .
# 6) ./Executable

cmake_minimum_required(VERSION 3.20)

project(Cmake4 VERSION 1.0.0 LANGUAGES C CXX)

# set placeholders
set(EXECUTABLE_NAME Executable)
set(LIBRARY_NAME Library)

# Tell cmake where to search for other cmake files!!!
# src file must come first! because we link library in our main.cpp
# Src -> Headers -> Main

add_subdirectory(src)
add_subdirectory(headers)
add_subdirectory(entryPoint)