cmake_minimum_required(VERSION 3.22)
project(robotiq_arg85_description)

find_package(ament_cmake REQUIRED)

ament_package()

#############
## Install ##
#############

install(DIRECTORY launch/
  DESTINATION share/${PROJECT_NAME}/launch)

install(DIRECTORY meshes/
  DESTINATION share/${PROJECT_NAME}/meshes)

install(DIRECTORY robots/
  DESTINATION share/${PROJECT_NAME}/robots/)

install(FILES urdf.rviz
  DESTINATION share/${PROJECT_NAME})


