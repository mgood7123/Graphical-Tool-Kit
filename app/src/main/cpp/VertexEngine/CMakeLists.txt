# For more information about using CMake with Android Studio, read the
# documentation: https://d.android.com/studio/projects/add-native-code.html

# Sets the minimum version of CMake required to build the native library.

cmake_minimum_required(VERSION 3.10.2)

# Declares and names the project.

project(VertexEngine)

add_library(
        VertexEngine SHARED
        VertexEngine.cpp
)

target_link_libraries(
        VertexEngine
        DiligentLibrary
        PixelToNDC
        WINAPI::Kernel
)
