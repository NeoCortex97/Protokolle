cmake_minimum_required(VERSION 3.10...3.16)

project(simple_command)

include(build/conanbuildinfo.cmake)
conan_basic_setup(TARGETS)

add_executable(simple_command src/main.cpp)
# target_link_libraries(simple_command )
