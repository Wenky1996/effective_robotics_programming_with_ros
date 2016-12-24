# Effective Robotics Programming with ROS - Third Edition #

[**Effective Robotics Programming with ROS - Third Edition**](https://www.packtpub.com/hardware-and-creative/effective-robotics-programming-ros-third-edition)'s book tutorials source code.

<a href="https://www.packtpub.com/hardware-and-creative/effective-robotics-programming-ros-third-edition"><img src=https://www.packtpub.com/sites/default/files/5576.jpg width=200/></a>

## Authors ##

* [Anil Mahtani](https://github.com/Anilm3)
* [Luis Sánchez](https://github.com/LuisSC)
* [Aaron Martinez](https://github.com/AaronMR)
* [Enrique Fernández](https://github.com/efernandez)

## Installation ##

Install **ROS Kinetic** on a compatible **Ubuntu** distro following the official instructions provided [here](http://wiki.ros.org/kinetic/Installation/Ubuntu).

Install the OpenCV non-free repository:

``` bash
sudo apt-get install software-properties-common python-software-properties
sudo add-apt-repository --yes ppa:xqms/opencv-nonfree
sudo apt-get install libopencv-nonfree-dev libopencv-nonfree2.4v5
```

Create a workspace:
``` bash
mkdir -p ~/dev/catkin_ws/src
cd ~/dev/catkin_ws/src
wstool init
```

Download this repository:
``` bash
wstool set ros_book --git git@github.com:rosbook/effective_robotics_programming_with_ros.git
wstool up -j8
```

Install the dependencies:
``` bash
cd ..
rosdep install --from-paths src -iy
```

Build the source code (alternatively, you can use `catkin build` instead of `catkin_make`):
``` bash
source /opt/ros/$(rosversion -d)/setup.bash
catkin_make -j4
source devel/setup.bash
```

## Tutorials ##

* **Chapter  1:** Getting started with ROS (no source code as it covers the installation)
* **Chapter  2:** ROS Architecture and Concepts
* **Chapter  3:** Visualization and Debugging Tools
* **Chapter  4:** 3D Modeling and Simulation
* **Chapter  5:** The Navigation Stack - Robot Setups
* **Chapter  6:** The Navigation Stack - Beyond Setups
* **Chapter  7:** Manipulation with MoveIt!
* **Chapter  8:** Using Sensors and Actuators with ROS
* **Chapter  9:** Computer Vision
* **Chapter 10:** Point Clouds
