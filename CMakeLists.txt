# CMake root file for duilib related apps
#Date 2012-09-16
#Author: Qi Gao(monkgau@gmail.com)
#
#  CMake files for duilib
#  file for each app is under the related sub-dir
#

cmake_minimum_required(VERSION 3.16)

project(dui LANGUAGES C CXX)

# this line is for UNICODE release,which is required by DuiDesigner 
# add_definitions(-DUNICODE -D_UNICODE)

add_compile_options("$<$<C_COMPILER_ID:MSVC>:/utf-8>")
add_compile_options("$<$<CXX_COMPILER_ID:MSVC>:/utf-8>")

# add each CMake file
add_subdirectory(duilib)
add_subdirectory(360SafeDemo)
add_subdirectory(FlashDemo)
add_subdirectory(GameDemo)
add_subdirectory(ListDemo)
add_subdirectory(QQDemo)
add_subdirectory(RichListDemo)
add_subdirectory(TestApp1)
