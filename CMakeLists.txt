cmake_minimum_required(VERSION 3.16)

project(dui LANGUAGES C CXX)

add_compile_options("$<$<C_COMPILER_ID:MSVC>:/utf-8>")
add_compile_options("$<$<CXX_COMPILER_ID:MSVC>:/utf-8>")

add_subdirectory(duilib)
# add_subdirectory(FileTree)
add_subdirectory(FlashDemo)
add_subdirectory(GameDemo)
add_subdirectory(ListDemo)
# add_subdirectory(MenuDemo)
add_subdirectory(QQDemo)
add_subdirectory(RichListDemo)
add_subdirectory(ScrCapture)
add_subdirectory(360SafeDemo)
add_subdirectory(TestApp1)
