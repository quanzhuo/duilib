add_executable(MenuDemo WIN32
    About.cpp
    About.h
    debug.cpp
    debug.hpp
    main_frame.cpp
    main_frame.hpp
    main.cpp
    MenuDemo.rc
    MenuNotify.cpp
    MenuNotify.h
    observer_impl_base.hpp
    resource.h
    SkinSetting.cpp
    SkinSetting.h
    StdAfx.cpp
    StdAfx.h
    UICrack.cpp
    UICrack.h
    UIMenu.cpp
    UIMenu.h
)

target_link_libraries(MenuDemo
    PRIVATE duilib
)

target_include_directories(MenuDemo
    PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})