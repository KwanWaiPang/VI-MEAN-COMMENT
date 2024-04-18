cmake_minimum_required(VERSION 2.8.3)
project(chisel_ros)


#设置使用c++14
ADD_COMPILE_OPTIONS(-std=c++14 ) #添加了编译选项，指定了 C++ 标准为 C++14。
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fexceptions" ) #设置了 C 编译器的额外编译选项，启用了异常处理。
set(CMAKE_CXX_STANDARD 14) #设置了 C++ 标准为 C++14
set(CMAKE_CXX_STANDARD_REQUIRED ON) #设置了 C++ 标准的强制要求为开启状态。
set(CMAKE_CXX_EXTENSIONS OFF) #关闭了 C++ 扩展
# 设置了 C++ 编译器的额外编译选项，包括启用调试信息、优化级别为 O3、链接了一些库等。
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g -std=c++14 -g -O3 -ltbb -lboost_system -msse2 -msse3 -pthread -w") # -Wall
 
if (DEFINED CATKIN_TOPLEVEL OR (NOT ("$ENV{ROS_DISTRO}" STREQUAL "fuerte")))
    include(${PROJECT_SOURCE_DIR}/catkin.cmake)
else ()
    include(${PROJECT_SOURCE_DIR}/rosbuild.cmake)
endif ()
