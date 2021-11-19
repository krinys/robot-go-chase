# robot-go-chase
RoboticsND_GoChaseIt
This is repository for the second project of Udacity Robotics Software Engineer Nanodegree.

It includes two ROS packages:

my_robot package - holds my robot, the white ball, and my world;
ball_chaser package - includes drive_bot and process_image nodes.
How to try them out?

Create a catkin_ws
$ cd /home/
$ mkdir -p /home/catkin_ws/src/
$ cd catkin_ws/src/
$ catkin_init_workspace
$ cd ..

Clone the packages in catkin_ws/src/
$ cd /home/catkin_ws/src/
$ git clone https://github.com/NataliyaMish/RoboticsND_GoChaseIt.git master
Build the packages
$ cd /home/catkin_ws/ 
$ catkin_make

After building the packages, source your environment
$ cd /home/catkin_ws/
$ source devel/setup.bash

Once the packages have been built, you can launch my_robot using
$ roslaunch my_robot world.launch

To launch drive_bot and process_image nodes, use
$ roslaunch ball_chaser ball_chaser.launch
Make robot chase the ball!
Just outside of the world you will see a white ball. Place it in front of the robot and see it moving towrds it! To stop robot, move the ball outside of its field of view.
