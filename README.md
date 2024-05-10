## Requirements
The following code is executed in ROS Noetic in Ubuntu 20.04 LTS

The following libraries are required to be installed before proceeding to run the code

    $ sudo apt-get install ros-noetic-turtlebot3*
    $ sudo apt-get install ros-noetic-gmapping
    $ sudo apt-get install ros-noetic-navigation
    $ sudo apt-get install python-opencv
    $ sudo apt-get install python-numpy
    $ sudo apt-get install python-scikits-learn
    $ sudo apt-get install ros-noetic-teb-local-planner
    $ sudo apt-get install ros-noetic-multirobot-map-merge


## Installation Process
Create a new folder called "ros_workspace/src" by executing the following comment:

    $ mkdir -p ~/ros_workspace/src
    $ cd ~/ros_workspace/src/
    $ git clone https://github.com/ignmercam/RRSS_MULTIPLE_SLAM.git
    $ cd ~/ros_workspace
    $ catkin_make



## Execution for Multirobot
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
