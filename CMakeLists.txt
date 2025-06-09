cmake_minimum_required(VERSION 3.31)
project(ResRover)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "/opt/homebrew/opt/qt")

find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(ResRover main.cpp)
target_link_libraries(ResRover
        Qt::Core
        Qt::Gui
        Qt::Widgets
)

