cmake_minimum_required(VERSION 2.8.3)

include(cmake/HunterGate.cmake)
HunterGate(
    URL "https://github.com/lsolanka/hunter/archive/v0.19.210-6.tar.gz"
    SHA1 "f41d25b617ecb7e7062b9f30648e50eae39f9475"
)

project(ros_comm)
hunter_add_package(ros-catkin)
hunter_add_package(ros-message_generation)
hunter_add_package(ros-message_runtime)
hunter_add_package(ros-std_msgs)

add_subdirectory(rosgraph_msgs)
add_subdirectory(std_srvs)
