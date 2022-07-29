cmake_minimum_required(VERSION 3.0)
project(gr-example CXX C)

add_subdirectory(dep/gnuradio)

add_executable(main main.cpp)
target_link_libraries(main gnuradio-analog gnuradio-audio gnuradio-blocks)
