cmake_minimum_required(VERSION 3.14.4)
project(servoarm_description)


find_package(ament_cmake REQUIRED)


install(FILES arm.urdf DESTINATION share/${PROJECT_NAME})

install(
  DIRECTORY meshes
  DESTINATION share/${PROJECT_NAME}/
)

ament_package()
