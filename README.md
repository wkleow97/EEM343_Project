# EEM343_Project
Dual arm robot for plant inspection

Assuming you have ROS, MoveIt! and Gazebo installed, catkin workspace created

For demo purpose

Copy the whole folder into src directory of catkin workspace

Open terminal, direct into catkin_ws:
cd catkin_ws

Source for ROS:
source devel/setup.bash

Start gazebo, spawn table and robot:
roslaunch test1_gazebo test1_gazebo.launch

start camera:
rosrun image_view image_view image:=/test1/camera1/image_raw

start rviz planning execution:
roslaunch test1_moveit_config test1_planning_execution.launch

spawn pot (left):
rosrun gazebo_ros spawn_model -file `rospack find pot`/urdf/pot.urdf -urdf -x -0.07615 -y -0.19943 -z 1 -model pot


