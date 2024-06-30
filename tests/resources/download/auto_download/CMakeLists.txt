cmake_minimum_required(VERSION 3.24)
project(MyApp CXX)

find_package(hello REQUIRED)
add_executable(app main.cpp)
target_link_libraries(app hello::hello)
