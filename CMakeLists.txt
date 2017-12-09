cmake_minimum_required(VERSION 2.8.3)

include(cmake/HunterGate.cmake)
HunterGate(
    URL "https://github.com/lsolanka/hunter/archive/ros-hunter.tar.gz"
    SHA1 "ae50a419e022bda5b6cb563dcab5b52f75daa44b"
)

project(ros_comm)
hunter_add_package(catkin)
hunter_add_package(message_generation)
hunter_add_package(message_runtime)
hunter_add_package(std_msgs)

add_subdirectory(rosgraph_msgs)
add_subdirectory(std_srvs)
