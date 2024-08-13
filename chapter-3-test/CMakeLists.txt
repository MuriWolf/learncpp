cmake_minimum_required(VERSION 3.16)

project(chapter-3-test LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(chapter-3-test main.cpp)

include(GNUInstallDirs)
install(TARGETS chapter-3-test
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
