cmake_minimum_required(VERSION 2.8.3)
project(ball_chaser)

add_compile_options(-std=c++11)

find_package(catkin REQUIRED COMPONENTS
  message_generation
  roscpp
  std_msgs
)


## Generate services in the 'srv' folder
add_service_files(
  FILES
  DriveToTarget.srv
)

## Generate added messages and services with any dependencies listed here
generate_messages(
  DEPENDENCIES
  std_msgs
)

## Specify additional locations of header files
## Your package locations should be listed before other locations
include_directories(
  ${catkin_INCLUDE_DIRS}
)

add_executable(drive_bot src/drive_bot.cpp)

add_dependencies(drive_bot ball_chaser_generate_messages_cpp)

## Specify libraries to link a library or executable target against
target_link_libraries(drive_bot  ${catkin_LIBRARIES})

