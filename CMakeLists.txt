cmake_minimum_required(VERSION 3.22)
project(robotiq_arg85_description)

find_package(ament_cmake REQUIRED)

ament_package()

#############
## Install ##
#############

install(DIRECTORY launch/
  DESTINATION share/${PROJECT_NAME})

install(DIRECTORY meshes/
  DESTINATION share/${PROJECT_NAME})

install(DIRECTORY robots/
  DESTINATION share/${PROJECT_NAME})

install(FILES urdf.rviz
  DESTINATION share/${PROJECT_NAME})


