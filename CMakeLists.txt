cmake_minimum_required(VERSION 2.8)

project(simple-web-server)

add_compile_options(
    -std=c++11
)

add_executable(final
    main.cpp
    optparse.cpp
    httpparser.cpp
    webserver.cpp)
target_link_libraries(final pthread)