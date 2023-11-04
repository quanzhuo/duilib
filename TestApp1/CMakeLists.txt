add_executable(TestApp1 WIN32 App.cpp
                              StdAfx.cpp
                              StdAfx.h)

target_link_libraries(TestApp1 PRIVATE duilib)
target_include_directories(TestApp1 PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})