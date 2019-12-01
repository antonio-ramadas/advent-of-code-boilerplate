cmake_minimum_required(VERSION 3.12)
project(advent-of-code-2018)

set(CMAKE_CXX_STANDARD 14)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR})

# From https://stackoverflow.com/a/7788165
# Get all subdirectories that start with "day-"
MACRO(SUBDIRLIST result curdir)
    FILE(GLOB children RELATIVE ${curdir} ${curdir}/day-*)
    SET(dirlist "")
    FOREACH(child ${children})
        IF(IS_DIRECTORY ${curdir}/${child})
            LIST(APPEND dirlist ${child})
        ENDIF()
    ENDFOREACH()
    SET(${result} ${dirlist})
ENDMACRO()

# All subdirectories are now at SUBDIRS
SUBDIRLIST(SUBDIRS ${CMAKE_SOURCE_DIR})

# Add each one
FOREACH(subdir ${SUBDIRS})
    ADD_SUBDIRECTORY(${subdir})
ENDFOREACH()
