cmake_minimum_required (VERSION 3.9)

include (../../src/common.cmake)

project (a.out)

add_executable(
  a.out
  main.cpp
)

target_link_libraries(
  a.out
  "-framework CoreFoundation"
  "-framework IOKit"
  "-framework SystemConfiguration"
)
