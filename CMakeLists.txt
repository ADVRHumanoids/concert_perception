cmake_minimum_required(VERSION 3.0)
project(concert_perception)

add_compile_options(-std=c++14)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  sensor_msgs
  std_msgs
  nav_msgs
  tf
  tf_conversions
  eigen_conversions
  geometry_msgs
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES perception_thesis_gap
  CATKIN_DEPENDS roscpp geometry_msgs sensor_msgs std_msgs tf tf_conversions
#  DEPENDS system_lib
)
