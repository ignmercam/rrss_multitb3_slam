TERMINAL 1
$ roscore

TERMINAL 2
$ source ~/ros_workspace/devel/setup.bash
$ export TURTLEBOT3_MODEL=waffle_pi
$ roslaunch rrss multiple_tb3_house.launch

TERMINAL 3
$ source ~/ros_workspace/devel/setup.bash
$ export TURTLEBOT3_MODEL=waffle_pi
$ roslaunch rrss two_robots.launch
