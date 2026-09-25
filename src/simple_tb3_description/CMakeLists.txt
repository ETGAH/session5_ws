cmake_minimum_required(VERSION 3.8)
project(simple_tb3_description)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY
    urdf
    launch
  DESTINATION share/${PROJECT_NAME}
)

ament_package()