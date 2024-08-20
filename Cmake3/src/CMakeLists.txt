# src CMake File

add_library(Library STATIC Starter.cpp)

# Tell cmake where to find the header files
target_include_directories(Library PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")