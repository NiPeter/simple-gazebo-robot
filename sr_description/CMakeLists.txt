cmake_minimum_required(VERSION 2.8.3)
project(sr_description)

find_package(catkin REQUIRED)

catkin_package(
  CATKIN_DEPENDS robot_state_publisher xacro
)

install(DIRECTORY
  launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)

install(DIRECTORY
  urdf/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/urdf
)
