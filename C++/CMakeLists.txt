cmake_minimum_required(VERSION 3.11)

project(pylon-samples)

# Find Pylon
find_library(PYLON pylon)
if (NOT PYLON)
    message(FATAL_ERROR "PYLON not found")
else()
    set(PYLON_INCLUDE_DIRS
        ${PYLON}/Headers
        ${PYLON}/Headers/GenICam)
        
    message(STATUS "Found PYLON")
endif()

#Add subdirs
add_subdirectory(Grab_UsingBufferFactory)