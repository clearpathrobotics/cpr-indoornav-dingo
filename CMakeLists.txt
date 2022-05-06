cmake_minimum_required(VERSION 3.0.2)
project(cpr_indoornav_dingo)

find_package(catkin REQUIRED)

catkin_package(
)

include_directories(
)

install(PROGRAMS
  scripts/environment
  scripts/install
  scripts/dingo_power_monitor
  scripts/start_dingo_bridge

  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)

install(DIRECTORY config img launch urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
