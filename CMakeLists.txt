cmake_minimum_required(VERSION 3.5)
project(aaveq_ros_interfaces)

set(CMAKE_CXX_STANDARD 20)

# Dependencies
find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)
find_package(std_msgs REQUIRED)
find_package(geometry_msgs REQUIRED)

# Interfaces
rosidl_generate_interfaces(${PROJECT_NAME}
    "msg/ControlOutput.msg"
    "msg/SimState.msg"
  DEPENDENCIES std_msgs geometry_msgs
 )

if(BUILD_TESTING)
  find_package(ament_lint_auto REQUIRED)
  ament_lint_auto_find_test_dependencies()
endif()

ament_package()
