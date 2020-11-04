
cmake_minimum_required (VERSION 3.8)

project ("TEST")

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include_directories("${CMAKE_SOURCE_DIR}/includes")
link_directories("${CMAKE_SOURCE_DIR}/lib")

add_executable(main main.cpp)

target_link_libraries(main PRIVATE "libaswl-shared-debug.lib")