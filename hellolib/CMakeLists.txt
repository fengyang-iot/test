
message(STATUS  "before in hellolib SRC_LIST = ${SRC_LIST}" )
file(GLOB SRC_LIST src/*.cpp)
message(STATUS  "after in hellolib SRC_LIST = ${SRC_LIST}" )
add_library(hellolib STATIC ${SRC_LIST})
target_include_directories(hellolib PUBLIC include)