add_executable(ListDemo WIN32 Main.cpp)
target_link_libraries(ListDemo duilib)
target_include_directories(ListDemo PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})