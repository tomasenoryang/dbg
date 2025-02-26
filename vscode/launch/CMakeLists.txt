cmake_minimum_required(VERSION 3.10)
project(launch)
set(CMAKE_CXX_STANDARD 17)

set(DBG_SOURCE_FILES main.cc)

add_executable(${PROJECT_NAME} ${DBG_SOURCE_FILES})

