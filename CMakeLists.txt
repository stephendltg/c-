# Cmake version
cmake_minimum_required(VERSION 3.0.0)
# Name's project and version
project(cpp-template VERSION 0.1.0)

include(CTest)
enable_testing()

# Header's files.
set (HEADERS
)

# Source's files
set (SOURCES
    main.cpp
)

# C++17
set (CMAKE_CXX_STANDARD 17)
# Build from files declare on SOURCES et HEADERS.
add_executable (cpp-template ${SOURCES} ${HEADERS})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
