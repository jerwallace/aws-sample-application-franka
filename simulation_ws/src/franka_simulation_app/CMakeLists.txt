cmake_minimum_required(VERSION 2.8.3)
project(franka_simulation_app)

find_package(catkin REQUIRED COMPONENTS
  panda_simulation
)

catkin_package()

install(DIRECTORY launch worlds
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
