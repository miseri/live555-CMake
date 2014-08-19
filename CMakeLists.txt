cmake_minimum_required(VERSION 2.6)

PROJECT( live555 )

SET(EXECUTABLE_OUTPUT_PATH ${live555_SOURCE_DIR}/bin)
SET(LIBRARY_OUTPUT_PATH ${live555_SOURCE_DIR}/lib)
SET(RUNTIME_OUTPUT_DIRECTORY ${live555_SOURCE_DIR}/bin)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${live555_SOURCE_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${live555_SOURCE_DIR}/bin)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${live555_SOURCE_DIR}/bin)

# includes
SET(live555Includes
${live555_SOURCE_DIR}/live/BasicUsageEnvironment/include
${live555_SOURCE_DIR}/live/groupsock/include
${live555_SOURCE_DIR}/live/liveMedia/include
${live555_SOURCE_DIR}/live/UsageEnvironment/include
)

ADD_SUBDIRECTORY( live ) 
