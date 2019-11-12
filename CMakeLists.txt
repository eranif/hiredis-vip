project(hiredis-vip)
include_directories(adapters)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -std=c99 -Wall")

FILE(GLOB SRCS "*.c")
add_library(hiredis_shared SHARED ${SRCS})
add_library(hiredis_static STATIC ${SRCS})