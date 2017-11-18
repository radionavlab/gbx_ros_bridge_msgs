## GBX-ROS-Bridge-Msgs
This package contains no source code. All it does is build the message definitions so other ROS packages can utilize them.

## Using this package
1) Clone this package in the same catkin workspace as the packages that need these messages.

2) For every package that requires these messages, edit the package.xml and add:
    ``` <build_depend>gbx_ros_bridge_msgs</build_depend> ```
    ``` <run_depend>gbx_ros_bridge_msgs</run_depend> ```

3) For every package that requires these messages, edit the CMakeLists.txt and add:
    a)  gbx_ros_bridge_msgs to find_package
    b)  gbx_ros_bridge_msgs to CATKIN_DEPENDS in catkin_package
    c)  add_dependencies(TARGET gbx_ros_bridge_msgs)