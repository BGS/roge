#####################################################################
# Root SDK level
#####################################################################
project(Roge_packman)
cmake_minimum_required(VERSION 2.6)
set(CMAKE_ALLOW_LOOSE_LOOP_CONSTRUCTS TRUE)
message(STATUS "Processing ${PROJECT_NAME}")

set(USE_CPP11 "yes")

######################################
# find libs
######################################
unset(MYCURL CACHE)
find_library(MYCURL NAMES curl)# HINTS ${MY_CURL_DIR} NO_DEFAULT_PATH)

include_directories(
"${PROJECT_SOURCE_DIR}/include"
)

add_subdirectory(src)
