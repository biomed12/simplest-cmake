cmake_minimum_required(VERSION 3.27)

set(CXX_STANDARD 20)

project(cpp-project)

find_package(Boost REQUIRED)
find_package(OpenSSL REQUIRED) 

add_executable(main main.cpp)
target_link_libraries(main OpenSSL::SSL)