cmake_minimum_required(VERSION 3.19.0 FATAL_ERROR)

set(GALI_PROG_NAME gali)
project(${GALI_PROG_NAME} LANGUAGES C CXX)

# ----- set general dirs -----

set(GALI_SOURCE_DIR "${CMAKE_SOURCE_DIR}/src")
set(GALI_BINARY_DIR "${CMAKE_SOURCE_DIR}/bin")

message("> source dir " ${CMAKE_SOURCE_DIR})
message("> binary dir " ${CMAKE_BINARY_DIR})

# ----- generate -----

add_subdirectory(${GALI_SOURCE_DIR})

# ----- set properties -----

set_target_properties(${GALI_PROG_NAME} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${GALI_BINARY_DIR})
