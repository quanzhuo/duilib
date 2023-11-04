add_executable(QQDemo WIN32 
    chat_dialog.cpp
    chat_dialog.hpp
    color_skin.cpp
    color_skin.hpp
    ColorPicker.cpp
    ColorPicker.hpp
    debug.cpp
    debug.hpp
    main_frame.cpp
    main_frame.hpp
    main.cpp
    observer_impl_base.hpp
    QQDemo.rc
    resource.h
    skin_change_event.hpp
    StdAfx.cpp
    StdAfx.h
    UIFriends.cpp
    UIFriends.hpp
    UIGroups.cpp
    UIGroups.hpp
    UIListCommonDefine.cpp
    UIListCommonDefine.hpp
    UIMicroBlog.cpp
    UIMicroBlog.hpp
)

target_link_libraries(QQDemo duilib)
target_include_directories(QQDemo PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})