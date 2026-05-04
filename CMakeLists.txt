cmake_minimum_required(VERSION 3.22)
project(SubLoop VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)

# Placeholder JUCE integration (user will link JUCE locally or via submodule)
# add_subdirectory(JUCE)

add_executable(SubLoop
    src/main.cpp
)
