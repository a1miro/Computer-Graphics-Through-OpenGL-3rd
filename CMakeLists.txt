cmake_minimum_required(VERSION 3.0.0)
project(through_opengl VERSION 0.1.0)

include(CTest)
enable_testing()

include_directories (/usr/local/include)
link_directories (/usr/local/lib)

option(BUILD_CHAPTER2 "Build Chapter2" ON)
if(BUILD_CHAPTER2)
    add_subdirectory(Chapter2)
endif()


set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
