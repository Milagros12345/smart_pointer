cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

add_executable(smart_pointer_test smart_pointer_test.cpp)

target_link_libraries(smart_pointer_test gtest_main)
target_link_libraries(smart_pointer_test gmock_main)

add_test(garbage_collector_test smart_pointer_test)
