cmake_minimum_required (VERSION 3.0)

project (cookieleak)

set(CMAKE_CXX_STANDARD 11)

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

#set(PISTACHE_INSTALL OFF)
#set(PISTACHE_BUILD_TESTS OFF)
#set(PISTACHE_ENABLE_NETWORK_TESTS OFF)
#set(PISTACHE_USE_SSL OFF)
#set(PISTACHE_BUILD_EXAMPLES OFF)
#add_subdirectory("${PROJECT_SOURCE_DIR}/extern/pistache" EXCLUDE_FROM_ALL)
#include_directories("${PROJECT_SOURCE_DIR}/extern/pistache/include")

add_executable(cookieleak src/main.cc)

#target_link_libraries(cookieleak pistache_static Threads::Threads)
