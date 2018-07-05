# Cubli Robot

* Author: Songyan XIN <xinsongyan@gmail.com>
* License: GNU General Public License, version 3 (GPL-3.0)

Cubli Robot simulation environment with ROS and Gazebo.

## Description

Simple robot with 4 link: a cube as base link and three cylinder wheel connected to the cube with continuous rotational joint. 


## Quick Start


Gazebo:

    roslaunch cubli_gazebo cubli_world.launch

ROS Control (position or torque control):

    roslaunch cubli_control cubli_position_control.launch
    
    (roslaunch cubli_control cubli_torque_control.launch)
  

Example of Moving Joints:

    rostopic pub /cubli/joint_x_position_controller/command std_msgs/Float64 "data: 0.5"

