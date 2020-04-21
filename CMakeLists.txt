project(cmake_test_project) # Required
cmake_minimum_required(VERSION 3.0) # Required. 3.0 is a good start.
# These are the bare minimum of a project

# add_subdirectory(src) # In CMake, everything is a string
message(STATUS "|||||||||||| ${PROJECT_SOURCE_DIR}")

# Added second folder just to illustrate how you add secondary folders
include_directories(${PROJECT_SOURCE_DIR}/src
		    ${PROJECT_SOURCE_DIR}/secondFolderEtc)

add_subdirectory(${PROJECT_SOURCE_DIR}/src) # You can also use variables
# PROJECT_SOURCE_DIR is a standard environment variable for Cmake

enable_testing()
add_subdirectory(tests) # just as a remidner you can do it this way
