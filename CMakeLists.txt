cmake_minimum_required(VERSION 3.0.2)
project(uwb_ins_eskf_msgs)

find_package(catkin REQUIRED COMPONENTS 
  message_generation
  std_msgs 
  geometry_msgs
)

add_message_files(DIRECTORY msg)

generate_messages(DEPENDENCIES 
  std_msgs 
  geometry_msgs
)

catkin_package(
  CATKIN_DEPENDS
  std_msgs
  message_runtime 
  std_msgs
)