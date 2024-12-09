cmake_minimum_required(VERSION 3.5)

project(spirals LANGUAGES C)

set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_C_FLAGS "-Wall -Wextra -pedantic -ansi")

add_executable(parser
    src/main.c
    src/parse.c
    src/table/table.c
    src/simplex.c
    src/input.txt
)