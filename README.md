# Introduction

Ever wanted to explore what’s beneath the river Brahmaputra or what secrets our delightful lakes are hiding. If yes, then welcome to team antahsagri where we find answers to these questions through our remotely operated vehicle, Antahsagari. Our team works on diverse modules from ROV designing to its navigation, incorporating image processing and a versatile framework ROS.

<p align="center">
  <img src="https://scontent.fixr1-1.fna.fbcdn.net/v/t1.0-0/p180x540/87168843_1406226076246389_6672358876907569152_o.jpg?_nc_cat=101&_nc_sid=110474&_nc_ohc=IAyL5wX5IqkAX9X6gN0&_nc_ht=scontent.fixr1-1.fna&_nc_tp=6&oh=833e10a8637677822bc62130d7015098&oe=5F320F34">
</p>


## AIM:

- The aim of the project is to basically explore underwater world.
- We are trying to analyse the impact of urbanisation on structure and function of river system using the chemical data extracted from the water using sensors.
- It can also be used as a survey platforms to map sea floor or characterise physical, chemical, biological properties of water.
- It can be used to perform infrastructure inspections of pipeline systems so that divers are not put in harm's way.


## Physical architecture:

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

## Methodology

We are using ArduSub which works seamlessly with Ground Control Station software that can monitor vehicle telemetry and perform powerful mission planning activities. It also benefits from other parts of the ArduPilot platform, including simulators, log analysis tools, and higher level APIs for vehicle management and control.ArduSub is the 'brains' of the ROV. The Raspberry Pi Companion Computer runs software that relays communications between the autopilot and QGroundControl via Ethernet communications. The Companion software also streams HD video to QgroundControl. We are using SITL for simulation.SITL is a simulator that allows you to run ArduSub without any hardware.

Below is a typical diagram of hardware components on the ROV and their connections.
<p align="center">
  <img src="https://www.ardusub.com/images/hardware-diagram.png">
</p>

