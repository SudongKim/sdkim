cmake_minimum_required(VERSION 3.14)
set(PRJ_NAME "CMAKE_TEST")
PROJECT(${PRJ_NAME})
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
enable_testing()

add_subdirectory(googletest-1.14.0)
add_subdirectory(Code)
add_subdirectory(tests)

# set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
# add
# include(GoogleTest)

# add_executable(
#   test_project
#   hello.cpp
# )
# target_link_libraries(
#   test_project
#   GoogleTest
# )


