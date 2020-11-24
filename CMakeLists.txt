cmake_minimum_required(VERSION 3.12)
project(BotServer)
include_directories(src/headers)

set(HEADERS "src/headers/*.h")
FILE(GLOB SOURCES src/*.cpp)
add_executable(BotServer ${SOURCES})

set(CMAKE_CXX_STANDARD 17)

target_link_libraries(BotServer)
