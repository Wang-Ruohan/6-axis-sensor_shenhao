cmake_minimum_required(VERSION 2.8.3)
project(111)

find_package(catkin REQUIRED COMPONENTS
  roscpp
)

include_directories(
  include ${catkin_INCLUDE_DIRS}
)

link_directories(
  ${catkin_LIB_DIRS} lib
)

add_executable(FTSensors ${PROJECT_SOURCE_DIR}/FTSensors.cpp )

# add_dependencies(viscosity ${${PROJECT_NAME}_EXPORTED_TARGETS} ${catkin_EXPORTED_TARGETS})
