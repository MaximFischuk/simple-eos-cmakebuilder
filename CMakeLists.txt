cmake_minimum_required(VERSION 3.10)

project( ProjectName )

list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/CMakeModules")

set( CMAKE_CXX_STANDARD 14 )
set( CMAKE_CXX_EXTENSIONS ON )
set( CXX_STANDARD_REQUIRED ON)

set( CLI_CLIENT_EXECUTABLE_NAME cleos )
set( GUI_CLIENT_EXECUTABLE_NAME eosio )

set(CMAKE_EXPORT_COMPILE_COMMANDS "ON")

include(wasm)

add_subdirectory(contracts)
