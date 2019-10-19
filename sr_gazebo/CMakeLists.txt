cmake_minimum_required(VERSION 2.8.3)
project(sr_gazebo)

find_package(catkin REQUIRED)

catkin_package(
  CATKIN_DEPENDS controller_manager gazebo_ros sr_description
)

install(DIRECTORY
  cfg/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/cfg
)

install(DIRECTORY
  launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)

install(DIRECTORY
  worlds/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/worlds
)
