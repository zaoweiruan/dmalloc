cmake_minimum_required(VERSION 3.10)
project(malloc VERSION 2.86)

add_library(malloc)
target_include_directories(malloc PUBLIC include)
set_target_properties(${PROJECT_NAME} PROPERTIES SOURCES "src/malloc.c")
set_target_properties(${PROJECT_NAME} PROPERTIES ARCHIVE_OUTPUT_DIRECTORY "${PROJECT_SOURCE_DIR}/bin")
set_target_properties(${PROJECT_NAME} PROPERTIES RUNTIME_OUTPUT_DIRECTORY "${PROJECT_SOURCE_DIR}/bin")

#target_link_libraries(malloc PUBLIC stdc++fs)