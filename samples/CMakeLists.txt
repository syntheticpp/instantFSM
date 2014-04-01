cmake_minimum_required(VERSION 2.8)

project(instantFSM-samples)

include_directories(
  ..
)

enable_testing()

add_executable(audioPlayer audioPlayer.cpp)

if (UNIX)
  target_link_libraries(audioPlayer stdc++)
endif (UNIX)

