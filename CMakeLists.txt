cmake_minimum_required(VERSION 3.29.0)
project(planning
VERSION 0.0.1 
DESCRIPTION "a demo"
HOMEPAGE_URL "https://github.com/xianyu925/NJU_game-main"
LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 17)

#变量和目录设置
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin) # 动态库和exe都指定到bin目录下
set(Process_Dir ${CMAKE_SOURCE_DIR}/src/process)
set(PNC_Map_Dir ${CMAKE_SOURCE_DIR}/src/pnc_map)

#添加子目录
add_subdirectory(src)