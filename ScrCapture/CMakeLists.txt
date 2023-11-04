add_executable(ScrCapture WIN32
    App.cpp
    Canvas.cpp
    Canvas.h
    CanvasContainer.cpp
    CanvasContainer.h
    ScrCaptureWnd.h
    ScrCaptureWnd.cpp
    StdAfx.h
    StdAfx.cpp
    Util.cpp
    Util.h
)

target_link_libraries(ScrCapture
    PRIVATE duilib
)

target_include_directories(ScrCapture
    PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})