cmake_minimum_required(VERSION 3.10)
project(PlotVisualGL)

set(CMAKE_CXX_STANDARD 14)




find_package(OpenGL REQUIRED)
find_package(glfw3 REQUIRED)

include_directories(${OPENGL_INCLUDE_DIR})



add_executable(PlotVisualGL main.cpp)
target_link_libraries(PlotVisualGL ${OPENGL_gl_LIBRARY} glfw)