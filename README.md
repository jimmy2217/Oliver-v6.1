# Oliver-v6.1 - 6 DOF Articulated Robot
Purpose of this robot is to create a medium payload high accuracy, high torque articulated robot arm from scratch to aquire new skills further cement complex kinematics control.

Key upgrades from previous version:
- BLDC high torque motors
- High speed, high power motor drivers (ODrive)
- Fully closed loop control (position, velocity, and torque)
- Hard-stop homing routines (no sensors)
- All aluminum construction
- Brakes added to joint 2 & 3
- USB2.0 high speed communication
- Utilizing RoboDK for teaching and IK solving

Skill aquired from v6.1:
- CAD to CAM workflow
- CNC machining 
- Advanced multi-threading process (python)
- High speed passthrough position and velocity control
- True linear end effector trajectory (work in progress)
- Online target teaching

# Motors Encoders and Drivers
Sensorless high torque hobby BLDC motors

![image](https://user-images.githubusercontent.com/55325587/148709207-4519504b-9112-4e30-9131-a9ad66d03018.png)

High resolution incremental encoders

![image](https://user-images.githubusercontent.com/55325587/148709379-b271030a-42a1-4138-82f8-86fd686f3972.png)

High power motor driver (ODrive)

![image](https://user-images.githubusercontent.com/55325587/148717887-0c697da7-bf38-4aa0-9fd9-8686e6d9d934.png)

# CAD design
![image](https://user-images.githubusercontent.com/55325587/148711787-d9e50060-dc86-4460-9cda-001b346d3020.png)
![image](https://user-images.githubusercontent.com/55325587/148711831-b03b40c5-8dbb-4902-baab-ee4a6222510d.png)
![image](https://user-images.githubusercontent.com/55325587/148711867-e4a884e8-ea5c-4537-b9bf-4beb52826086.png)

# CAM workflow and all aluminum structure machined on Bantam Tools Desktop CNC Machine
https://user-images.githubusercontent.com/55325587/148712347-256cf629-7926-46bf-919e-e067f01fabe6.mov

https://user-images.githubusercontent.com/55325587/148712499-92c2a46f-1eb4-4630-8cb2-8823a0c0d8e2.mov

https://user-images.githubusercontent.com/55325587/148716694-4f198a16-49a4-4282-a3c0-68bea7ef0a98.mov

# Python script and GUI

![image](https://user-images.githubusercontent.com/55325587/148720005-c26a18bc-d0ec-415a-9d17-e13406bdcabf.png)

![image](https://user-images.githubusercontent.com/55325587/148716939-0ca03f1c-43da-4e4e-96b3-4b1b49d96679.png)

![image](https://user-images.githubusercontent.com/55325587/148716965-482a8a1e-1e7c-48f9-8c77-fbfe7f24d8c1.png)

![image](https://user-images.githubusercontent.com/55325587/148717308-d787a7ba-4271-4056-9f6d-1be441ff7856.png)

# Hard-Stop (no sensor) homing procedure

The hard-stop (no limit sensors or switches) homing relys on continuously monitoring motor current and setting a "homing current limit" that is used to stop motion when the joint physically hits the end of its range of motion. When this happends, the joint is then moved to its "home" position based on the IK model created for the robot.
In the image below, notice the spike in motor current when the hard-stop is located.

![image](https://user-images.githubusercontent.com/55325587/148717610-ff44b4ef-8ed4-451b-b922-5915ff4ebf38.png)

[![Capture](http://img.youtube.com/vi/XPeweSGB3SE/0.jpg)](https://www.youtube.com/watch?v=XPeweSGB3SE)

[![Capture](http://img.youtube.com/vi/zMl4PU84S9U/0.jpg)](https://www.youtube.com/watch?v=zMl4PU84S9U)

[![Capture](http://img.youtube.com/vi/vJOct1IJHY0/0.jpg)](https://www.youtube.com/watch?v=vJOct1IJHY0)

# Online programming and target teaching

https://user-images.githubusercontent.com/55325587/148718598-4b6d81ec-a1ce-48eb-a527-24667ea97618.mov

https://user-images.githubusercontent.com/55325587/148718860-4ed7613e-1484-42f8-9be3-8f410d00dee5.mov

# Position, Velocity and torque tuning

![image](https://user-images.githubusercontent.com/55325587/148719832-830e9497-88d7-4225-85ac-00194d555420.png)

![image](https://user-images.githubusercontent.com/55325587/148719852-63e830fc-20ef-4ab5-bd22-f7b68efd5a39.png)

https://user-images.githubusercontent.com/55325587/148719860-4c23d3f7-3684-49bb-b2d7-11d6fd0565ca.mov


