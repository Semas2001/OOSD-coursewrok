cmake_minimum_required(VERSION 3.1)

project(test)

set(SFML_DIR "C:/SFML/lib/cmake/SFML")

find_package(SFML 2.5.1 COMPONENTS system window graphics audio network REQUIRED)

add_executable(test Pacman.cpp)

target_link_libraries(test sfml-system sfml-window sfml-graphics sfml-audio sfml-network )