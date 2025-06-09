cmake_minimum_required(VERSION 3.14)
project(SimpleDrawingApp)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_OSX_ARCHITECTURES "arm64")

find_package(Qt6 REQUIRED COMPONENTS Widgets)

add_executable(SimpleDrawingApp MACOSX_BUNDLE main.cc)

target_link_libraries(SimpleDrawingApp Qt6::Widgets)