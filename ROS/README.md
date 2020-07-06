# Getting Started

Work Done:
-All sensors values publishing through ROS node
-Video streaming capture with OpenCV using ROS
-Arming and setting Flight mode.
-Locomotion control using Keyboard and Servo Control, integrated with ROS
-Getting all the data of ROV state using ROS.



## Brushing up ROS Skills
The Robot Operating System (ROS) is a flexible framework for writing robot software.ROS is a software suite which allows for quick and easy building of autonomous robotic systems. ROS should be considered as a set of tools for creating new solutions or adjusting already existing ones. A major advantage of this system is a great set of drivers and implemented algorithms widely used in robotics.
First of all, it's a good idea to read through the official ROS [tutorials](http://wiki.ros.org/ROS/Tutorials) before going forward.
For a quick revision go through this [link](https://docs.google.com/document/d/1ldGKymQ69mHqShosXWEiA1hdclQTj8zcJI4iImfuoGE/edit?usp=sharing).

### Requirements ###

-Git
-ROS Melodic Version installed on UBUNTU 18.04 LTS
-Python 
 -OpenCV
 -[Pymavlink](https://www.ardusub.com/developers/pymavlink.html)
 -[pynput](https://pypi.org/project/pynput/)
 -[gi, gobject](https://wiki.ubuntu.com/Novacut/GStreamer1.0)
 -mavros
-QGroundControl

  -Firstly, downl0oad [QGroundControl](https://docs.qgroundcontrol.com/en/getting_started/download_and_install.html#ubuntu) for Linux and enter all the commands in the terminal corrresponding to #####Ubuntu Linux Section

-SITL
 -To configure and run SITL for the first time in your computer, take a look in [Running SITL](http://ardupilot.org/dev/docs/sitl-simulator-software-in-the-loop.html) ArduPilot documentation.
Please follow the instructions in [Setting up the Build Environment (Linux/Ubuntu)](https://ardupilot.org/dev/docs/building-setup-linux.html#building-setup-linux) to set up the full environment, including SITL.
-Also, proficiency on using ardusub and  mavlink messages is required

### Installation of ROS Package ###
 1. Go to your ROS package source directory:
    - `$ cd ros_workspace_path/src`
 2. Clone this project.
 3. Go back to your ROS workspace:
    - `$ cd ../`
 4. Build and install it:
    - `$ catkin_make --pkg parameters`
 5. Reload your ROS env.
    - bash: `$ source devel/setup.sh`
    - zsh: `$ source devel/setup.sh`


### Running with SITL and QGC ###
- Run ArduPilot SITL


    1. `$ cd ardupilot/ArsuSub`
    2. `$  sim_vehicle.py -L RATBeach --out=udp:0.0.0.0:14550 --map --console`
    3. `$./QGroundControl.AppImage`
    4. `$ rosrun file_name.py`



## Some Commands ##

