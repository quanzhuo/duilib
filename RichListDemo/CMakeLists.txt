add_executable(RichListDemo WIN32 
  Resource.h
  RichListDemo.cpp
  RichListDemo.rc
  RichListDemo.h
  RichListDemo.ico
  RichListWnd.cpp
  RichListWnd.h
  stdafx.cpp
  stdafx.h
)

target_link_libraries(RichListDemo duilib)
target_include_directories(RichListDemo PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})