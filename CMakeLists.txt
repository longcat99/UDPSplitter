cmake_minimum_required(VERSION 3.10) # 更新为较新的版本
project(UDPSplitter LANGUAGES CXX)  # 声明使用 C++ 项目

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# 添加源文件
set(SOURCES 
    UDPSplitter.cpp
    AddressManager.cpp
)

set(HEADERS
    AddressManager.h
    AddressInfo.h
    CommandReceiver.h   # 添加新的头文件
)

# 添加可执行文件
add_executable(UDPSplitter ${SOURCES} ${HEADERS})

# 链接库
target_link_libraries(UDPSplitter pthread)
