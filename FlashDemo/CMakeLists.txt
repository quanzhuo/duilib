add_executable(FlashDemo WIN32 App.cpp StdAfx.cpp StdAfx.h)
target_link_libraries(FlashDemo duilib)
target_include_directories(FlashDemo PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})