cmake_minimum_required(VERSION 3.20)
project(Clickomania)

set(CMAKE_CXX_STANDARD 17)

SET(TARGET_H
        Grid.h
        GameState.h
        clickomania.h
        )
# Local source files here
SET(TARGET_SRC
        Grid.cpp
        GameState.cpp
        )


add_executable(Clickomania clickomania.cpp ${TARGET_SRC} ${TARGET_H} singlefile.cpp)
add_executable(Singlefile singlefile.cpp)
