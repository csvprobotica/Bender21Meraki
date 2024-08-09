## Bender21 Meraki WRO 2024
The independent team Bender21 Meraki is integrated by Juan David Castillo, Daiana Castilo and Karl Serrano in this Future Engineers competition.

Engineering materials
====

This repository contains engineering materials of a self-driven vehicle's model participating in the WRO Future Engineers competition in the season 2024.

Elements of our robot:
* 1 LEGO Mindstorms EV3 brick 45500
* 1 Rechargeable battery DC 2050mAh 45501
* 1 EV3 L-Servo Motor 45502
* 1 EV3 M-Servo Motor 45503
* 2 Technic Distance Sensor 45504
* 1 Technic Color Sensor 45506
* 1 Gyroscope Sensor 45505
* 3D modeling designs for assembly

## Content

* [`models`](https://github.com/csvprobotica/HypeTech/tree/main/models) in this directory you will find the 3D modeled files for the assembly of the robot and its components.
* [`other`](https://github.com/csvprobotica/HypeTech/blob/main/other/Flowchart.png) in this directory you will find additional files of the robot operation, process diagram and execution.
* [`schemes`](https://github.com/csvprobotica/HypeTech/tree/main/schemes) contains a schematic diagram in JPG format of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they are connected to each other.
* [`src`](https://github.com/csvprobotica/HypeTech/tree/main/src) contains code of control software for all components which were programmed to participate in the competition.
* [`t-photos`](https://github.com/csvprobotica/HypeTech/tree/main/t-photos) contains 2 photos of the team (an official one and one funny photo with all team members).
* [`v-photos`](https://github.com/csvprobotica/HypeTech/tree/main/v-photos) contains 6 photos of the vehicle (from every side, from top and bottom).
* [`video`](https://github.com/csvprobotica/HypeTech/tree/main/video) contains the video.mp4 file with the robot driving demonstration.

## Strategy and Mobility

**Robot Description:**

Our robot is an innovative autonomous machine designed for navigation and obstacle avoidance in its environment. It is equipped with a series of sensors and motors that allow it to detect and respond to various stimuli along its path.

**Proximity Sensors:**
The robot features several strategically placed proximity sensors around its structure. These sensors enable the detection of walls and other obstacles, ensuring that the robot can navigate without collisions. The sensors work by measuring the distance to nearby objects and providing real-time data to the robot's control system.

**Motors:**
* Front Motor: This motor is responsible for the robot's turns. Upon receiving signals from the control system, it can rotate in different directions, allowing the robot to avoid obstacles and redirect its path.
* Rear Motor: This motor drives the robot forward. It is designed to provide smooth and consistent movement, adjusting as needed based on the navigation requirements determined by the sensors.

**Color Sensor:**
The robot is also equipped with a color sensor capable of detecting specifically red and green colors. When encountering a red or green object in its path, the robot's control system activates an evasion routine to avoid these objects, ensuring safe and uninterrupted navigation.

**Gyroscope Sensor:**
To enhance its navigation capability and ensure it follows a precise trajectory, the robot includes a gyroscope sensor. This sensor measures the robot's orientation and turns. The control system uses gyroscope data to perform up to three complete turns before stopping. This feature is essential for tasks requiring cyclical navigation or following specific patterns.

**Functionality:**
Together, these components allow the robot to navigate autonomously and efficiently in complex environments. Upon starting, the robot moves forward, using its proximity sensor to detect walls and adjust its trajectory through controlled turns by the front motor. Simultaneously, it monitors its surroundings for red and green objects to evade them. The gyroscope ensures the robot can make precise turns and count up to three turns before stopping, completing its operation cycle.

## Programming Explained
In this section are placed the phases used in the programming based on the sequence of actions and responses of the robot in the detection in its sensors and motor movements during autonomous navigation.

**Phase 1:** Start and Initial Movement
- The robot begins its operation when the system starts. In this phase, the robot sets itself in motion and moves forward.
- The rear motor drives the robot forward.

**Phase 2:** Obstacle Detection
- As the robot moves forward, its proximity sensors scan the environment to detect potential obstacles, such as walls or other objects.
- The proximity sensors provide real-time data to the robot's control system.

**Phase 3:** Obstacle Avoidance
- Upon detecting an obstacle in its path, the robot uses its front motor to turn in the appropriate direction and avoid a collision.
- The front motor executes a turn to change the robot's direction, allowing it to continue moving without hitting the obstacle.

**Phase 4:** Specific Color Detection
- During navigation, the robot uses its color sensor to identify red or green objects in its path.
- If a red or green object is detected, the control system activates an evasion routine to maneuver around the object.

**Phase 5:** Gyroscope-Guided Navigation
- The robot's gyroscope measures its orientation and turns, ensuring it follows a precise trajectory.
- The robot performs up to three complete turns based on gyroscope data before stopping.

**Phase 6:** Completion of Operation Cycle
- After completing up to three turns, the robot concludes its operation cycle and stops.
- The control system powers down the motors, and the robot stops, completing the assigned task.
