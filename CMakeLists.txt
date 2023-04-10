cmake_minimum_required(VERSION 3.24 FATAL_ERROR)

project(cmake
    VERSION 0.0.1
    PROJECT_DESCRIPTION "The project description for CMake"
    CMAKE_PROJECT_HOMEPAGE_URL "https://github.com/sanyusily/CMakeProcessControl"
    LANGUAGE    "C CPLUSPLUS"
)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(BuildInfo)

add_subdirectory(src)
add_subdirectory(external)
add_subdirectory(docs)
add_subdirectory(package)
add_subdirectory(example)