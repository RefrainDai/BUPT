cmake_minimum_required(VERSION 3.30)

project(HelloWorld)

add_library(HW
    src/HW.cpp
)


add_executable(main
    src/main.cpp
)
target_link_libraries(main HW)
target_include_directories(main PRIVATE include)
