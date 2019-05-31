cmake_minimum_required(VERSION 2.6)
project(bwa)

set(CMAKE_CXX_COMPILER /usr/bin/gcc)

add_custom_target(BWA cd ${PROJECT_SOURCE_DIR} && make VERBATIM)
add_custom_target(BWA-clean cd ${PROJECT_SOURCE_DIR} && make clean VERBATIM)
