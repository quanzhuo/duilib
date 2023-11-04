# #Cmake file for QQDemo
# #Author: Qi Gao(monkgau@gmail.com)
# #Created: 2012/9/17

# aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} SRC)
# include_directories(${CMAKE_CURRENT_SOURCE_DIR})                           


# set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
# add_executable(QQDemo ${SRC} QQDemo.rc)
# set_target_properties(QQDemo PROPERTIES LINK_FLAGS "/SUBSYSTEM:WINDOWS")
# target_link_libraries(QQDemo duilib)


# add_custom_command(TARGET QQDemo POST_BUILD
#   COMMAND ${CMAKE_COMMAND} -E copy_if_different
#   ${PROJECT_BINARY_DIR}/bin/QQDemo.exe ${PROJECT_SOURCE_DIR}/bin/QQDemo.exe)

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