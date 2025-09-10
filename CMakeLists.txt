# --- Basic Project Setup ---
# Set the minimum version of CMake required
cmake_minimum_required(VERSION 3.10)

# Define the project name, version, and languages
project(
    debugging
    VERSION 0.1.0
    DESCRIPTION ""
    LANGUAGES CXX)

if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)

    # Set the C++ standard to C++17. This ensures modern features are available.
    set(CMAKE_CXX_STANDARD 17)
    set(CMAKE_CXX_STANDARD_REQUIRED ON)

    # Ensure using -std=c++xx instead of -std=gnu++xx
    set(CMAKE_CXX_EXTENSIONS OFF)

    # Enables folders in IDEs that support it
    set_property(GLOBAL PROPERTY USE_FOLDERS ON)

    include(FetchContent)
    FetchContent_Declare(
        googletest
        URL https://github.com/google/googletest/archive/03597a01ee50ed33e9dfd640b249b4be3799d395.zip
    )

    FetchContent_MakeAvailable(googletest)

    # Include testing
    enable_testing()
    include(CTest)
    include(GoogleTest)
    add_subdirectory(tests)

endif()

# Compiled library is here
add_subdirectory(src)

# Exe code is here
add_subdirectory(apps)