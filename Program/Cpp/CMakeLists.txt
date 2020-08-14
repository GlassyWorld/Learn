cmake_minimum_required(VERSION 3.0)

# 项目名称
project(Test)

set(CMAKE_C_COMPILER "gcc")
set(CMAKE_CXX_COMPILER "g++")
set(CMAKE_CXX_STANDARD 11)

# 根目录/代码路径
aux_source_directory(. DIR_MAIN)

# debug 模式
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g")

# 编译可执行文件
set (EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR})
add_executable(${PROJECT_NAME} ${DIR_MAIN}) 