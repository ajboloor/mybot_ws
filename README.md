## Platform for testing ROS and Gazebo

- ROS Version: Kinetic
- Gazebo Version: 7.11

Based on https://github.com/richardw05/mybot_ws.git

## Terminal Commands:

- ./run_gazebo - launch gazebo world with mybot robot
- ./run_cmd - give linear and angular velocity to robot for circular motion
- ./run_rviz - visualization of robot with sensors in rviz

## Requirements:
```
sudo apt-get install ros-kinetic-gazebo

sudo apt-get install ros-kinetic-turtlebot ros-kinetic-turtlebot-apps ros-kinetic-turtlebot-
interactions ros-kinetic-turtlebot-simulator ros-kinetic-kobuki-ftdi ros-kinetic-ar-track-
alvar-msgs

sudo apt-get install ros-kinetic-slam-gmapping 

sudo apt-get install ros-kinetic-turtlebot-teleop
```
