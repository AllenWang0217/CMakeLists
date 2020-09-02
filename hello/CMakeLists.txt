set(curr_dir ${CMAKE_CURRENT_SOURCE_DIR})

include_directories(
    include
)

aux_source_directory(${curr_dir}/source DIR_HELLO_SRCS)

add_library(hello ${DIR_HELLO_SRCS})