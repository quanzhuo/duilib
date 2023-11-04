add_executable(GameDemo WIN32 GameDemo.cpp MiniDumper.cpp StdAfx.cpp GameDemo.rc)
target_link_libraries(GameDemo duilib)
target_include_directories(GameDemo PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})