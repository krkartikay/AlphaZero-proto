cmake_minimum_required(VERSION 2.8.12)

project(omega)

include_directories(.)
include_directories(include)

add_compile_options(-std=c++17)

# if(CMAKE_CXX_FLAGS_DEBUG)
#    set (CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -fno-omit-frame-pointer -fsanitize=address,undefined")
#    set (CMAKE_LINKER_FLAGS_DEBUG "${CMAKE_LINKER_FLAGS_DEBUG} -fno-omit-frame-pointer -fsanitize=address,undefined")
# endif(CMAKE_CXX_FLAGS_DEBUG)

file(GLOB SOURCES "src/*.cpp")

add_executable(omega ${SOURCES})