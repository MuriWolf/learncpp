cmake_minimum_required(VERSION 3.16)

project(chapter-2-test LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(chapter-2-test main.cpp
    io.h io.cpp
)

include(GNUInstallDirs)
install(TARGETS chapter-2-test
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
