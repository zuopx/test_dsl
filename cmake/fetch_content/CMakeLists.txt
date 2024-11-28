#
# mkdir build; cmake ..
#


cmake_minimum_required(VERSION 3.14)
project(MyProject)

include(FetchContent)
message("FETCHCONTENT_BASE_DIR=${FETCHCONTENT_BASE_DIR}")
# ${CMAKE_BINARY_DIR}/_deps: /root/project/test_dsl/cmake/fetch_content/build

FetchContent_Declare(
  googletest
  URL https://github.com/google/googletest/archive/03597a01ee50ed33e9dfd640b249b4be3799d395.zip
)
FetchContent_MakeAvailable(googletest)
message("FETCHCONTENT_BASE_DIR=${FETCHCONTENT_BASE_DIR}")
