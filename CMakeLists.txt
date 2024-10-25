cmake_minimum_required(VERSION 3.0)

project(LoggerProject)

# 设置包含头文件目录和源文件目录
set(LOG_INCLUDE_DIR include)
set(LOG_SOURCE_DIR src)

# 添加可执行文件
add_executable(logger ${LOG_SOURCE_DIR}/main.cc)

# C++11 标准
set_target_properties(logger PROPERTIES CXX_STANDARD 11 CXX_STANDARD_REQUIRED ON CXX_EXTENSIONS OFF)  