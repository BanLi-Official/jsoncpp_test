cmake_minimum_required(VERSION 3.28.2)
project(main)

include_directories(${include})

link_directories(${lib})
link_libraries(jsoncpp)

aux_source_directory(${PROJECT_SOURCE_DIR} source)

set(EXECUTABLE_OUTPUT_PATH  ${out})

add_executable(main ${source})