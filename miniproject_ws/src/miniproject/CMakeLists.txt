cmake_minimum_required(VERSION 2.8.3)
project(miniproject)

find_package(catkin REQUIRED COMPONENTS roscpp rospy std_msgs geometry_msgs)

catkin_package()

add_executable(pubvel pubvel.cpp)
target_link_libraries(pubvel ${catkin_LIBRARIES})


include_directories(
  ${catkin_INCLUDE_DIRS}
)

