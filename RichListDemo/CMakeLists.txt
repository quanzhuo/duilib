# #Cmake file for RichListDemo
# #Author: Qi Gao(monkgau@gmail.com)
# #Created: 2012/9/17

# aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} SRC_LIST)
# include_directories(${CMAKE_CURRENT_SOURCE_DIR})                           


# set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)

# add_executable(RichListDemo ${SRC_LIST} RichListDemo.rc)
# set_target_properties(RichListDemo PROPERTIES LINK_FLAGS "/SUBSYSTEM:WINDOWS")
# target_link_libraries(RichListDemo duilib)

# add_custom_command(TARGET RichListDemo POST_BUILD
#   COMMAND ${CMAKE_COMMAND} -E copy_if_different
#   ${PROJECT_BINARY_DIR}/bin/RichListDemo.exe ${PROJECT_SOURCE_DIR}/bin/RichListDemo.exe)

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