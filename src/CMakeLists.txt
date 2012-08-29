#####################################################################
# test Project
#####################################################################
project(roge)
message(STATUS "Processing ${PROJECT_NAME}")


#####################################################################
# Include the project files
#####################################################################
FILE(GLOB HEADER_FILES "*.h")
FILE(GLOB SOURCE_FILES "*.cpp")

#####################################################################
# Set to build as an executable
#####################################################################
add_executable(${PROJECT_NAME} ${HEADER_FILES} ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME} ${MYCURL})
