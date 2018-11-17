cmake_minimum_required (VERSION 3.0)
project(example VERSION 1.0 LANGUAGES C)
include(${CMAKE_CURRENT_LIST_DIR}/DefineFindPackage2.cmake)

define_find_package2(ZSTD zstd.h zstd)
find_package2(ZSTD)
add_executable(example example.c)
target_link_libraries(example PRIVATE ZSTD::ZSTD)

# vim: ts=4 sw=4 sts=4 et
