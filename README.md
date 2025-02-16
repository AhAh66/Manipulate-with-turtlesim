# Manipulate-with-turtlesim
# Manipulating the `turtlesim` Package in ROS Noetic/Melodic

## Prerequisites
Ensure you have **ROS Noetic** or **ROS Melodic** installed

## draw a squere
![AWLinux  Running  - Oracle VM VirtualBox 2_15_2025 1_52_06 PM](https://github.com/user-attachments/assets/294d7d04-27b7-4bbf-9b88-d7e312914dbd)


## 1. Launch the Turtlesim Node

First, start `roscore` in a terminal:
```sh
roscore
```
Then, open a new terminal and run:
```sh
rosrun turtlesim turtlesim_node
```

## 2. Control the Turtle Using Keyboard
To manually control the turtle, run:
```sh
rosrun turtlesim turtle_teleop_key
```
Use arrow keys to move the turtle.

## 3. Move the Turtle Using Commands
You can publish velocity commands to control the turtle:
```sh
rostopic pub /turtle1/cmd_vel geometry_msgs/Twist -r 1 -- '[2.0, 0.0, 0.0]' '[0.0, 0.0, 1.5]'
```
This command moves the turtle forward while rotating.
