# erwhi-hedgehog-ros
ERWHI Hedgehog ROS files

## Setup
Go into your workspace source folder (e.g. catkin_ws/src): <br>
`cd ~/catkin_ws/src` <br>
clone this repository: <br>
`git clone http://github.com/gbr1/erwhi-hedgehog-ros.git` <br>
return in catkin_ws: <br>
`cd ..` <br>
check dependencies: <br>
`rosdep install --from-paths src --ignore-src -r -y` <br>
make: <br>
`catkin_make` <br>
install: <br>
`catkin_make install` <br>

## Launch
Let's start Erwhi: <br>
`roslaunch erwhi_bringup bringup.launch` <br>
To simulate in Gazebo: <br>
`roslaunch erwhi_gazebo erwhi_gazebo.launch` <br>
To run autonomous navigation: <br>
`roslaunch erwhi_navigation explore.launch` <br>

## Dependencies
* [sengi_ros](https://github.com/gbr1/sengi_ros)
* [bosch_imu_driver](https://github.com/gbr1/bosch_imu_driver)
* [realsense2_camera](https://github.com/intel-ros/realsense)

## Known issues
* teb_local_planner configurations are not finals, at the moment Erwhi works on DWA.
* frontier_exploration configurations need to be fixed.


__Copyright (c) 2019 Giovanni di Dio Bruno under MIT license__
