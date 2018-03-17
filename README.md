<p align="center">
  <img src="/media/simple_maze_ros.gif">
</p>


## Platform for testing ROS and Gazebo

- ROS Version: Kinetic
- Gazebo Version: 7.11

Based on https://github.com/richardw05/mybot_ws.git

## Terminal Commands:

- ./run_gazebo - launch gazebo world with mybot robot
- ./run_cmd - give linear and angular velocity to robot for circular motion
- ./run_rviz - visualization of robot with sensors in rviz

Grab willow_garage.pgm (107 MB) from https://drive.google.com/open?id=19qgc33GMiKADq-p_aDTKzgeXyQ7PxEfF for learned willow garage map.

## Requirements:
```
sudo apt-get install ros-kinetic-gazebo-ros

sudo apt-get install ros-kinetic-turtlebot ros-kinetic-turtlebot-apps ros-kinetic-turtlebot-
interactions ros-kinetic-turtlebot-simulator ros-kinetic-kobuki-ftdi ros-kinetic-ar-track-
alvar-msgs
```
## Notes:
- Changes to CMakeLists may be required before catkin_make
- Above recorded simulation is speed up 10 times

## Usage: 
### Terminal 1 (Gazebo): 
```
roslaunch mybot_gazebo mybot_world.launch
```
### Terminal 2 (Map Building):
```
roslaunch mybot_navigation amcl_demo.launch
```
### Terminal 3 (Rviz):
```
roslaunch mybot_description mybot_rviz_amcl.launch
```
- Use 2D Nav Goal in Rviz to Navigate
