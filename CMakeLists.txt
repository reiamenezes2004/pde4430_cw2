cmake_minimum_required(VERSION 3.0.2)
project(assessment2)

find_package(catkin REQUIRED COMPONENTS
    roscpp
    rospy
    std_msgs
    gazebo_ros
)

catkin_package()

include_directories(
    ${catkin_INCLUDE_DIRS}
)

install(DIRECTORY launch worlds models scripts
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

