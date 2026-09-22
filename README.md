# Session 5 - URDF, TF, Gazebo and RViz

This repository contains the training files used in Session 5 of the TurtleBot3 workshop.

## Package

simple_tb3_description

## Included

- Simplified TurtleBot3 URDF
- Training-copy URDF for safe fault exercises
- RViz launch workflow
- robot_state_publisher
- joint_state_publisher for offline training only

## Important

The training URDF is a simplified teaching model.

Do not treat its dimensions as the exact production TurtleBot3 Burger dimensions.

Do not use joint_state_publisher as a competing joint-state source on the physical TurtleBot3.

## Build

From the repository root:

source /opt/ros/jazzy/setup.bash

colcon build --symlink-install

source install/setup.bash

## Launch the good model

ros2 launch simple_tb3_description display.launch.py

## Launch the training model

ros2 launch simple_tb3_description training_display.launch.py

## Validation

check_urdf src/simple_tb3_description/urdf/simple_tb3.urdf