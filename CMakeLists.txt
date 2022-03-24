cmake_minimum_required(VERSION 2.8 C)

set(PROJECT_NAME b64c)

set(B64_INCLUDES ${CMAKE_CURRENT_SOURCE_DIR} PARENT_SCOPE)


add_library(${PROJECT_NAME} STATIC
    buffer.c
    decode.c
    encode.c
)

target_include_directories(${PROJECT_NAME} INTERFACE .)
