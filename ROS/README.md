# Getting Started

### Physical architecture:

Antahsagri  is an under-water remotely operated vehicle (ROV), designed to explore the underwater world and collect data for research and analysis. It is equipped with several sensors:

- 6 Thrusters T100
- 6 Basic Esc
- 1 Bar30 pressure sensor
- 1 Temperature Sensor
- 2 Leak sensors
- 2 Lumen Subsea Lights
- 1 Raspberry Pi , used as a companion computer
- 1 camera
- 1 servo for the camera tilt
- 1 PixHawk with internal 9 DOF IMU

The small size of the Antahsagri and its high manoeuvrability is perfect to achieve exploration missions in tiny places. Also, its wide variety of sensors make the automation easier.


## Brushing up ROS Skills
The Robot Operating System (ROS) is a flexible framework for writing robot software.ROS is a software suite which allows for quick and easy building of autonomous robotic systems. ROS should be considered as a set of tools for creating new solutions or adjusting already existing ones. A major advantage of this system is a great set of drivers and implemented algorithms widely used in robotics.
First of all, it's a good idea to read through the official ROS [tutorials](http://wiki.ros.org/ROS/Tutorials) before going forward.
For a quick revision go through this [link](https://docs.google.com/document/d/1ldGKymQ69mHqShosXWEiA1hdclQTj8zcJI4iImfuoGE/edit?usp=sharing).


## ROS Architecture:
ROS is a robotic middleware, a collection of software framework for robot software development. This tool provide a great abstraction for client server
program. With ROS there is node, corresponding to the execution of the code and topics, a place that receive messages published from node. 

- Sensors on the robot collect valuable data of its surrounding and gives us a direct or indirect knowing of its physical state.
- These data are then sent and processed in the controller that will output a command for the actuators. The command evolves with time according to the desired         state and the current one.
- The main pros is that nodes can subscribe to topics to listen messages and publish on topics to share data with other nodes.

## MAVlink:
To communicate, the ROV used MAVlink witch is a lightweight messaging protocol design for drones and moving robots. To deal with this message, the
ROV runs Ardusub, a branch of ardupilot project for underwater vehicles on a Pixhawk, a hardware electronic card to easely connect sensors and pwm motors
with MAVlink. On the topside computer, the software QGroundControl is made for handling MAVlink message, conjure Ardusub on the ROV.

## Ardusub:

The ArduSub project is a fully-featured open-source solution for remotely operated underwater vehicles (ROVs) and autonomous underwater vehicles (AUVs). ArduSub is a part of the ArduPilot project, and was originally derived from the ArduCopter code. ArduSub has extensive capabilities out of the box including feedback stability control, depth and heading hold, and autonomous navigation.

ArduSub works seamlessly with Ground Control Station software that can monitor vehicle telemetry and perform powerful mission planning activities. 

