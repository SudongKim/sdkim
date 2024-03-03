CMAKE_MINIMUM_REQUIRED(VERSION 3.14)

set (BINARY ${CMAKE_PROJECT_NAME})
set (EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR})
set(LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR})

set (src_files hello.cpp )

#add_executable( ${BINARY}_run ${src_files})
add_library( ${BINARY}_lib STATIC ${src_files})
