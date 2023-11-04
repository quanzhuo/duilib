add_executable(FileTree WIN32 
    FileTree.cpp
    FileTree.h
    FileTree.rc
    MainDialog.cpp
    MainDialog.h
    Resource.h
    StdAfx.cpp
    StdAfx.h
    targetver.h
)

target_link_libraries(FileTree
    PRIVATE duilib
)

target_include_directories(FileTree
    PRIVATE
        ${CMAKE_CURRENT_SOURCE_DIR})