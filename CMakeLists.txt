cmake_minimum_required(VERSION 3.10)

#Enter your project name.
project("main")

add_executable("${PROJECT_NAME}" "src/main.cpp")

install(TARGETS "${PROJECT_NAME}" DESTINATION bin)