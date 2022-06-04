cmake_minimum_required(VERSION 3.1)

project(05-singleton)

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)
add_executable(05-singleton main.cpp)
target_link_libraries(05-singleton PRIVATE Threads::Threads)