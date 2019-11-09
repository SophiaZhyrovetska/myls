cmake_minimum_required(VERSION 3.14)
project(myls)

set(CMAKE_CXX_STANDARD 14)
find_package(Boost REQUIRED COMPONENTS filesystem program_options)

add_executable(myls main.cpp myfile.cpp myfile.hpp)

target_link_libraries(myls ${Boost_LIBRARIES})