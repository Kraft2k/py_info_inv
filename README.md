# py_info_inv

Invironment Setup
$ source /opt/ros/foxy/setup.bash


Create C++ package
$ ~/ros2_ws/src$ ros2 pkg create my_cpp_pkg --build-type ament_cmake –dependencies rclpp

Only CPP package
$ colcon build –packages-select my_cpp_pkg

Create new file
$ touch my_cpp_node.cpp

&&&&&
$ cat  ~/.bashrc

$ ros2 node list

$ ros2 node info /py_test

Rename a node at Runtime 
$ ros2 run my_py_pkg py_node  --ros-args –remap __node:=abc
$ ros2 run my_py_pkg py_node  --ros-args –r __node:=node2
