cmake_minimum_required (VERSION 3.5)

project(NMSISNNSVDF)

file(GLOB SRC "./*_*.c")

add_library(NMSISNNSVDF STATIC ${SRC})

### Includes
target_include_directories(NMSISNNSVDF PUBLIC "${NN}/Include")
target_include_directories(NMSISNNSVDF PUBLIC "${DSP}/Include")
