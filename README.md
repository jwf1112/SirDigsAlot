# LKRoverApp
The primary code for controlling the Lunar Knights Mars Mining Robot.

The Lunar Knights application will likely contain a few different packages.

//Needs Update
  
# Install dependencies
```

sudo apt-get install ros-kinetic-diff_drive_controller

sudo apt-get install ros-kinetic-controller_manager
//Needs update
```
# How to install

```
# create a folder to put the code in
mkdir -p ~/catkin_ws

# copy the repository into ~/catkin_ws/src
git clone https://github.com/LunarKnights/SirDigsAlot src/

# set up the catkin workspace
cd ~/catkin_ws/src
catkin_init_workspace

# build the project
source ~/catkin_ws/devel/setup.bash
cd ~/catkin_ws
catkin_make
```

# Developer notes
The code should be formatted against the ROS standard so that's everything's nice and uniform.
The easiest way to do this is using `clang-tidy` with this guy's [formatting rules](https://github.com/davetcoleman/roscpp_code_format)
You can add this as a precommit git so that it will automatically do all this for you by following these instructions

```
# TODO
```


## Order to read files
These are currently fully commented:
- lk\_rover/src/lk\_rover\_node.cpp
- lk\_rover/src/lk\_rover\_controller.cpp
- lk\_rover/src/lk\_rover.cpp
- lk\_rover/src/lk\_rover\_hw.cpp
- lk\_rover/src/gazebo\_hw.cpp
- arduino\_stuff/arduino\_motor\_controller/arduino\_motor\_controller.ino

## Useful references
http://wiki.ros.org/roscpp/Overview/Services
http://wiki.ros.org/roscpp/Overview/Publishers%20and%20Subscribers
http://wiki.ros.org/roscpp/Overview/Messages
http://gazebosim.org/tutorials?tut=ros_comm&cat=connect_ros
http://docs.ros.org/kinetic/api/gazebo_msgs/html/srv/JointRequest.html

