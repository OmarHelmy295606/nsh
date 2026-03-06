cmake_minimum_required(VERSION 3.10)
project(nsh)

add_executable(nsh
    src/main.cpp
    src/parser.cpp
    src/executer.cpp
    src/builtins.cpp
)

target_compile_features(nsh PRIVATE cxx_std_17)

target_include_directories(nsh PRIVATE include)
