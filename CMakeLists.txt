cmake_minimum_required(VERSION 3.16.3)
project(    
    lesson1                                 # название проекта                        
    VERSION 0.0.0                           # номер версии проекта
    DESCRIPTION "First project"             # описание           
    LANGUAGES CXX                           # язык программирования
)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_BUILD_TYPE Debug)

add_executable(lesson1)
#add_library(lesson1, SHARED)

set(sources
    body_program.cpp
)
target_sources(lesson1 PRIVATE ${sources})