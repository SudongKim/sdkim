set (BINARY ${CMAKE_PROJECT_NAME}_tst)
set (EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/build/tests)

FILE(GLOB_RECURSE test_source_list FALSE *.h *.cpp)
set(SOURCES ${test_source_list})

add_executable(${BINARY} ${test_source_list})
add_test(NAME ${BINARY} COMMAND ${BINARY})
target_link_libraries(${BINARY} PUBLIC ${CMAKE_PROJECT_NAME}_lib gtest)
include(GoogleTest)
gtest_discover_tests(${BINARY})
