cmake_minimum_required(VERSION 2.8.3)
project(sr_teleop)

find_package(catkin REQUIRED)

catkin_package(
  CATKIN_DEPENDS joy joy_teleop
)

install(DIRECTORY
   launch/
   DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)

install(DIRECTORY
  cfg/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/cfg
)
