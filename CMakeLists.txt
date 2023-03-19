cmake_minimum_required(VERSION 3.24)
project(hello)

set(CMAKE_CXX_STANDARD 17)

set(SFML_DIR "D:/myproject/SFML-2.5.1/lib/cmake/SFML")
find_package(SFML 2.5 COMPONENTS graphics audio REQUIRED)

add_executable(hello main.cpp)

# Link SFML library
target_link_libraries(hello sfml-graphics sfml-audio)
