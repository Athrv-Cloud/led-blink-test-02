cmake_minimum_required(VERSION 3.13)
project(LedBlinkTests)

# Include directories for STM32 and CppUTest
include_directories(src)

# Define an option to enable or disable the 'tests' directory
option(ENABLE_TESTS "Enable building tests" OFF)

# Add the 'tests' subdirectory only if ENABLE_TESTS is ON
if(ENABLE_TESTS)
    add_subdirectory(tests)
endif()
