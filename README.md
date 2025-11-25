# Content (GitHub)
**schemes** This folder contains one or several schematic diagrams in the form of JPEG, PNG, or PDF of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they connect. This folder also included the schematic diagram of the robot for both open and obstacle challenge.

**src** This folder contains all the programming flowcharts and all programming used to participate in the WRO 2025 Future Engineers Category.

**t-photos** This folder contains photos of the team participating in the WRO 2025 Future Engineers Category.

**v-photos** This folder contains photos of the vehicle from all sides (top view, bottom view, front view, back view and side views)

**video** This folder contains video.md file that demonstrates how the robot functions to solve both challenges.

**models** This folder contains the robot building insturction and the 3D printed part building instruction that installed on the vehicle. The file is presented in .lxf, .ldr and .ldr format.

**other** This folder contains other files which can be used to understand how to prepare the vehicle for the competition.

Here attached with the link for our **COMPLETE DOCUMENTATION MODULE** (https://drive.google.com/file/d/107QRZqFFLUvLz7qMj4gl7RzuqnLO4l_k/view?usp=sharing)

# Table of Contents (Essay)
- [Introduction](#introduction)
- [X-UniTech Team, Malaysia](#x-unitech-team-malaysia)
- [Performance video](#performance-video)

- [1.0 Mobility Management](#10-mobility-management)
  - [1.1 Design of the self-driving car](#11-design-of-the-self-driving-car)
  - [1.2 Chassis of the self-driving car](#12-chassis-of-the-self-driving-car)
  - [1.3 Building of the self-driving car](#13-building-of-the-self-driving-car)

- [2.0 Power and Sense Management](#20-power-and-sense-management)
  - [2.1 Power source](#21-power-source)
  - [2.2 Sensor](#22-sensor)
  - [2.3 Build Of Materials (BOM)](#23-build-of-materials-bom)
  - [2.4 Wiring diagram](#24-wiring-diagram)

- [3.0 Obstacles Management](#30-obstacles-management)
  - [3.1 Open Challenge](#31-open-challenge)
  - [3.2 Obstacle Challenge](#32-obstacle-challenge)

- [4.0 Engineering Factors](#40-engineering-factors)
  
- [5.0 Improvements and Enhancements](#50-improvements-and-enhancements)
  - [5.1 Robot Construction](#51-robot-construction)
  - [5.2 Robot Programming](#52-robot-programming)

- [Credits](#credits)

- [Appendix 1. The Building Instruction of the Self-Driving Car](#appendix-1-the-building-instruction-of-the-self-driving-car)
- [Appendix 2. Open Challenge Programming](#appendix-2-open-challenge-programming)
- [Appendix 3. Obstacle Challenge Programming](#appendix-3-obstacle-challenge-programming)

# Introduction
This engineering documentation details comprehensive aspects of the car’s mobility management, power and sensor systems, obstacle detection and avoidance, construction design, integration of third-party sensors, and the improvements that were made throughout our preparation for the **World Robot Olympiad (WRO) International Final in Singapore 2025** under the Future Engineers Category.


# X-UniTech Team, Malaysia
X-UniTech is a team from Malaysia consisting of three-member engineering team specializing in the development of autonomous vehicles. Our team is responsible for the end-to-end design, construction, and integration of the vehicle's mechanical and electronic systems to ensure optimal performance. Let’s meet our members:

**Vun Xiu Xuan, Alvin Kong Wei Ee, and Grace Tan Hong Hui.**

<img width="1020" height="764" alt="Team Photo" src="https://github.com/user-attachments/assets/9270f1dd-48bb-4caf-93c4-008a8048cd62" />

# Performance video
This video demonstrates our autonomous vehicle's design and its operational performance in both the Open Challenge and the Obstacle Challenge. Kindly scan the QR code below or access the link to watch the video for both challenges. https://youtu.be/pi9NsIusMks

<img width="250" height="250" alt="Performance Video (YouTube)" src="https://github.com/user-attachments/assets/e27dbd22-1fb4-488e-ad44-9704f637ad07" />

<img width="250" height="250" alt="Performance Video (Google Drive)" src="https://github.com/user-attachments/assets/9b49bde9-0131-4191-98f3-3d17b8937ec4" />

# 1.0 Mobility Management
This section details the **mechanical design and propulsion system of our autonomous vehicle.** It covers the **chassis construction, component layout, and the integration of the motors.** Additionally, it introduces the fundamental engineering principles of speed, torque, and power that govern the vehicle's performance.


## 1.1 Design of the self-driving car
The autonomous self-driving car chassis and mechanical structure are built using the **Lego 45544 Mindstorms EV3 Education Set and various third-party sensors** such as **Pixy2 Camera** and **EV3 Multiplexer.**

<img width="1920" height="1080" alt="Lego 45544 Mindstorms EV3 Education Set" src="https://github.com/user-attachments/assets/e4e4a845-6d69-4b65-a35b-6dd13c652df5" />


The figures below show the autonomous vehicle we designed and constructed.  


**Top view**	

<img width="1920" height="1080" alt="Robot (Top View)" src="https://github.com/user-attachments/assets/bc4a3e61-c65b-4ee0-93c7-85319cfcf775" />


**Bottom view** 

<img width="1920" height="1080" alt="Robot (Bottom View)" src="https://github.com/user-attachments/assets/c8b20f0e-9017-4c2f-8956-5c429a31611a" />


**Front view**	

<img width="1920" height="1080" alt="Robot (Front View)" src="https://github.com/user-attachments/assets/a4670633-ccd4-480d-9ede-2802662e1a39" />


**Back view** 

<img width="1920" height="1080" alt="Robot (Back View)" src="https://github.com/user-attachments/assets/fd65f990-3e34-4027-a636-42cb5d000160" />


**Left side view**	

<img width="1920" height="1080" alt="Robot (Left Side View)" src="https://github.com/user-attachments/assets/80207a5e-1eb6-45c8-8068-612a19bd2fc0" />


**Right side view** 

<img width="1920" height="1080" alt="Robot (Right Side View)" src="https://github.com/user-attachments/assets/a5b661ce-f8d7-4787-88ac-4b59aa907e47" />



## 1.2 Chassis of the self-driving car
The self-driving car chassis is designed to provide **structural support** and maintain **stability**, especially during high-speed maneuvers like sharp turns and rapid acceleration.


**(i) Selection of tyre**

For the front steering axle, we selected the **Medium Azure Hard Tyre** from the **Spike Essential** set because of its **hard rubber compound** that minimizes bouncing, allowing the vehicle **to track in a straight line** more reliably compared to softer tyres. The tyre's smaller diameter enables smoother and more precise steering corrections.

<img width="1920" height="1080" alt="Medium Azure Hard Tyres" src="https://github.com/user-attachments/assets/5f9d309f-d5bc-4d81-9f06-f58820d1f58c" />



The rear axle is fitted with **LEGO MINDSTORMS EV3 tyres** (62.4 x 20 mm) on 43.2 mm rims. These tyres were selected for the excellent traction their tread pattern provides on typical competition surfaces, such as floors and mats. This high-grip design prevents wheel slippage during rapid acceleration and high-speed cornering. 

<img width="1920" height="1080" alt="Lego Mindstorms EV3 Tyres" src="https://github.com/user-attachments/assets/b47b9379-f939-4589-8fa2-3fb2f7b2d223" />



**(ii) Implementation of motor and its engineering principle**

Our self-driving car propulsion system consists of two EV3 Medium Motors mounted in a compact, orthogonal arrangement (one horizontal, one vertical). This design offers several key advantages: it optimizes internal space, simplifies the gear train assembly, and contributes to a low center of gravity. A low center of gravity is crucial for maintaining stability during the high-speed maneuvers required in the Open Challenge. 

<img width="1920" height="1080" alt="EV3 Medium Motors" src="https://github.com/user-attachments/assets/82c9303f-119b-4e4c-b1ef-d426487d7c21" />


The diagram below illustrates the specifications and features of the EV3 Medium Motor.

<img width="914" height="559" alt="Specifications of EV3 Medium Motor" src="https://github.com/user-attachments/assets/5dbc4ca2-edca-4869-88de-54c19f1756f7" />


The vehicle's steering mechanism is controlled by an **EV3 Medium Motor**, selected for its high responsiveness and precision. With a running torque of **8 Ncm** and a stall torque of **15 Ncm**, the motor provides ample force for steering control. Furthermore, its rotational speed of **260 rpm** allows quick rotations, making it well-suited for fine adjustments when avoiding traffic signs. 

 **(iii) Implementation of differential gear**
 
A differential gear is integrated into the drive axle, allowing the left and right wheels to **rotate at different speeds.** This mechanism is essential for executing smooth, controlled turns, as it prevents wheel binding and improves stability. This is particularly critical when navigating the tight corners found in the Open Challenge. Not only that, our robot also incorporates **a step-up gear ratio.** This setup makes the wheels spin **1.29 times faster** than the motor, increasing the speed from **260 RPM** at the motor to about **335 RPM** at the wheels. This helps the robot to move faster while at the same time maintaining stability during tight turns.

<img width="1920" height="1080" alt="Differential Gear" src="https://github.com/user-attachments/assets/1c7cc38c-aca0-4bae-8c5e-5b6c5fcd4ea0" />



**(iv) Engineering principle of steering**

The steering system is designed using **Ackermann steering geometry.** 

<img width="1920" height="1080" alt="Ackermann Steering Geometry" src="https://github.com/user-attachments/assets/95865c69-4f91-40b5-b555-ee7da422e191" />



This principle **turns the inner front wheel at a sharper angle** than the outer wheel, allowing both to follow ideal concentric turning circles. By minimizing lateral tire scrub, this geometry significantly reduces friction and wear. The primary benefits include enhanced cornering stability, improved traction, and the ability to execute sharp turns with greater precision.


## 1.3 Building of the self-driving car
The **building instruction for the self-driving car** and the video of showcasing the **3D printing process** of its parts can be accessed via the QR Code and link below. 



**Building Instruction of Self-Driving Car (PDF format)**

<img width="250" height="250" alt="Building Instruction of Self-Driving Car (PDF Format)" src="https://github.com/user-attachments/assets/1248dd7f-9f1d-45a1-96fb-e42d79cac07e" />

https://drive.google.com/file/d/1kxk_LDarD3ZvdxKddqRiFiEe-euDLpLJ/view?usp=sharing



**3D Printing Process Video**

<img width="250" height="250" alt="3D Printing Process Video" src="https://github.com/user-attachments/assets/35378bb6-5235-4c56-966c-2b47691c22bf" />

https://youtu.be/b9eLe_nYFe0

# 2.0 Power and sense management
This section details the vehicle's **power source** and **sensor systems.** It covers the selection **rationale** and **implementation** of each sensor, along with an **analysis** of the **system's power consumption.** A **complete Build of Materials (BOM)** and **wiring diagram** are also provided for reference.

## 2.1 Power Source
The self-driving car is powered by a **Soshine 1.5V AA rechargeable lithium-ion (Li-ion) battery** with an energy capacity of 2600 mWh. This battery technology was selected for its stable voltage output, which ensures consistent and reliable performance for all electronic components.

<img width="1920" height="1080" alt="Soshine Rechargeable AA Lithium-Ion Battery" src="https://github.com/user-attachments/assets/e8abd1cd-4cb5-40e9-a2c1-207449a67023" />



## 2.2 Sensor
The self-driving car is designed to handle the diverse requirements of the Open and Obstacle Challenges. It includes **one color sensor, two ultrasonic sensors, one gyro sensor, and a Pixy2 camera.** The diagram below illustrates the placement and integration of these components.

<img width="860" height="465" alt="Sensors" src="https://github.com/user-attachments/assets/78331f56-3102-4a15-b7cd-ac550d0b374e" />



**(i) Pixy2 camera** 

The Pixy2 camera serves as the primary vision system for the vehicle during the Obstacle Challenge. Its main function is real-time object detection, allowing it to simultaneously **identify and track the red and green pillars** while the vehicle is in motion. It also helps to scan the magenta-colored parking zone to ensure the vehicle avoids this restricted area while navigating the course. The Pixy2 camera is mounted at a **65° angle** to provide optimal visibility when tracking traffic signs.

<img width="500" height="400" alt="Pixy2 Camera" src="https://github.com/user-attachments/assets/f3a4ec2f-25fe-405b-a306-32baf5eab139" />


<img width="500" height="400" alt="65° Pixy2 Camera" src="https://github.com/user-attachments/assets/19f715e7-009c-45e8-9d5f-7d7991dfc067" />




**(ii) Gyro sensor**

One gyro sensor is used to support our self-driving car. During both Open and Obstacle Challenge, it helps to **measure angles** and **maintain the correct heading** while driving. The gyro sensor also helps the robot to **turn at accurate angle** after passing the edge of the inner wall. While the gyro sensor can sometimes display errors at startup due to calibration issues, we resolved this by performing a hard reset before each run.

<img width="1920" height="1080" alt="Gyro Sensor" src="https://github.com/user-attachments/assets/bd85f198-947c-4ae1-a1b7-ebc95725d62f" />



**(iii) Ultrasonic sensor**

Our self-driving car is equipped with **two EV3 ultrasonic sensors.** These sensors measure the distance between the robot and wall **to avoid collision towards the walls.** The sensors operate by emitting sound waves and calculating the time it takes for them to bounce back after hitting a wall. This data enables the self-driving car to navigate efficiently, make accurate turns, and aim to complete the Open Challenge in the shortest time possible.

<img width="1920" height="1080" alt="Ultrasonic Sensor" src="https://github.com/user-attachments/assets/9b52f57b-6064-4ec2-942a-c995cfd6dd3c" />



**(iv) Color sensor**

The colour sensor is only used in the Obstacle Challenge to **determine when the self-driving car should turn.** In a **clockwise** direction, the car **turns right** whenever it detects an orange line, while in a **counterclockwise** direction, it **turns left** upon detecting a blue line. The sensor functions by measuring the intensity of light entering it, allowing the car to identify colour lines and determine whether it is moving clockwise or counterclockwise. 

<img width="1920" height="1080" alt="Color Sensor" src="https://github.com/user-attachments/assets/23ab26fb-c364-4723-88a9-22fc39e13672" />



## 2.3 Build of materials (BOM)

The table below shows the Build of Materials (BOM) used to build the self-driving car, making sure each part matches the car’s needs and functions.

![Build of Materials (1)](https://github.com/user-attachments/assets/9e9f3599-7feb-4877-87d8-f01668d08083)


![Build of Materials (2)](https://github.com/user-attachments/assets/e752d094-8206-4ed4-89d2-da396c3b617b)


![Build of Materials (3)](https://github.com/user-attachments/assets/2271334b-5652-4ce3-8639-68e5b48cc638)


![Build of Materials (4)](https://github.com/user-attachments/assets/851443a5-23d3-4921-a65a-7049e75b4071)


![Build of Materials (5)](https://github.com/user-attachments/assets/dd68a0f8-b9b2-4e3e-8c2e-168471174423)


![Build of Materials (6)](https://github.com/user-attachments/assets/f044b50f-3f4b-4e11-9e41-ac1782f832a8)



## 2.4 Wiring diagram
The wiring diagram below illustrates the **sensors’ power consumption** and shows how the **motors and sensors are connected** within our self-driving car to support the setups for both the Open Challenge and the Obstacle Challenge. 

**(i) Open challenge wiring diagram**

<img width="1920" height="1080" alt="Open Challenge Wiring Diagram" src="https://github.com/user-attachments/assets/917123b5-817e-4985-9e7c-a76ad723af4f" />



**(ii) Obstacle challenge wiring diagram**

<img width="1920" height="1080" alt="Obstacle Challenge Wiring Diagram" src="https://github.com/user-attachments/assets/9d8700f3-ab9e-44b7-9f4b-bbb29ec05ad4" />

# 3.0 Obstacles Management
In our project, we utilize the Clev3r-Python programming language to operate the robot. The programming structure is divided into two main sections which is the **Open Challenge** and the **Obstacle Challenge.** This section includes a flowchart and an overview of the code used for both challenges. 

## 3.1 Open Challenge
To complete the open challenge, our robot uses two main sensors which is an **EV3 Gyro Sensor** and **two EV3 Ultrasonic Sensors** on both the left and right sides. Since both **EV3 Ultrasonic Sensors** share the same port, we use a **multiplexer** to allow the robot to read data from each one separately. The left ultrasonic sensor is connected to Channel 2 of the multiplexer, while the right ultrasonic sensor is connected to Channel 3.

<img width="1920" height="1080" alt="Gyro Sensor and Ultrasonic Sensor" src="https://github.com/user-attachments/assets/45020216-7922-4002-a9a2-7f2c5fd4d31a" />



The **EV3 Ultrasonic Sensors** helps the car to measure the distance between the robot and the walls. By comparing readings from the left and right sensors, the robot can determine whether it should move clockwise or counter clockwise. These readings also help the robot adjust its steering to avoid collisions and stay at a safe distance from inner and the outer walls. Additionally, the **EV3 Gyro Sensors** monitor the robot’s heading, ensuring it maintains a straight path and performs accurate turns at the correct angle when turning. 

<img width="1920" height="1080" alt="Determine Direction (1)" src="https://github.com/user-attachments/assets/e06d8279-6bf6-4f5d-81e2-6127b51e55ca" />


In a quick overview, when the robot starts, it **first checks and sets up all its sensors.** Next, it **resets its steering** before moving. The robot then uses a **PID control system** to ensure smooth and stable turns. A drive function controls its speed and distance based on sensor data. Finally, the **main program** combines all these functions, enabling the robot to **follow walls, make precise turns,** and **complete all laps** efficiently and accurately. Further explanations of each function and programming part are provided in the **3.1.1 section below.**

Diagram below shows the flowchart for Open Challenge: 

<img width="475" height="680" alt="Open Challenge Flow Chart" src="https://github.com/user-attachments/assets/20ee63ea-7d1e-4a33-aedb-8a48f9da2328" />



**Appendix 2** contains the complete programming code for the **Open Challenge.**

### 3.1.1	Coding explanation
Below is a brief explanation of the key parts of the code used to control the robot during the challenge.

**(a)	Initialization and Setup**

This part is aim to set up the sensors and multiplexer before running. The **setMultiplexerMode function** allows the EV3 to connect with both ultrasonic sensors in the same port while the **getMultiplexerValues function** allows the robot to read the distance values from the left and right ultrasonic sensors. Additionally, the **ReadSensor** continuously updates the robot’s heading and wall distances in real time.

<img width="745" height="594" alt="Initialization and Setup" src="https://github.com/user-attachments/assets/a53ffbee-6a30-403d-b8af-f371a4b2d3f4" />



**(b) Car Position Coordinate Tracking**

This part of the program is about **position tracking using a gyro sensor and motor speed.** It continuously calculates the robot’s position on the X and Y axis based on how fast the motor is spinning and the angle detected by the gyro sensor. The **Math.Sin** and **Math.Cos** functions are used to determine the direction of movement, converting the robot’s rotation into **horizontal (x) and vertical (y)** changes. The program keeps updating these values in real time, showing them on the LCD screen. To prevent errors, it also limits both the X and Y positions to a **range between -20 and 20.** In simple terms, this part allows the robot to “know” where it is moving by combining speed and direction data, then displays its current position on the screen.

<img width="699" height="361" alt="Car Position Coordinate Tracking" src="https://github.com/user-attachments/assets/6b5248a6-df3a-4a7e-83ea-630813f52406" />


**(c) Reset Steering**

**Reset Steering** make sure the steering motor starts at a fixed desired position before driving. The robot turns the steering motor all the way to the left for **300 milliseconds** by using the **medium motor in the port A.** Hence, it waits until the motor completely stops moving, which means it has hit the limit. After that, the motor’s rotation is reset to zero. This step is important because it gives the information to the robot exactly where the “straight ahead” position is.

<img width="451" height="257" alt="Reset Steering" src="https://github.com/user-attachments/assets/60e26918-6d16-4a41-b185-4985d51db871" />



**(d) PID Steering Control**

The **PID Steering function** helps the robot to adjust the steering motor whenever it starts to drift off from the target. The **P** part fixes most of the error right away, the **I** part makes small adjustments over time and the **D** part make sure that the correction is done smoothly. These three adjustments are added together to get one correction value, which is sent to motor A to turn the steering. This keeps the robot moving smoothly, avoiding zig-zagging, and makes its turns more accurate.

<img width="717" height="362" alt="PID Steering function" src="https://github.com/user-attachments/assets/4a89c8e8-b752-47f0-b284-8f500dba621c" />



**(e) Drive**

Function **Drive** controls how the robot **drives and follows a wall.** First, it checks whether the ultrasonic sensors on both sides are working. If either sensor is not detecting a wall (value = 0), the robot **stops moving.** This acts as a **safety feature,** ensuring the robot doesn’t move blindly when there is no sensor data. If both sensors are working, the robot moves forward at the given speed.

  Next, when wall tracking (trackWall) is turned on, the robot adjusts its direction to stay at the correct distance from the wall. If the robot is moving **clockwise,** it uses the right sensor; if moving **counterclockwise,** it uses the left sensor. It calculates how much the robot **needs to turn** to maintain the proper distance and making sure it’s not too close or too far. If the error is **more than or less than 40** based on the robot’s distance and the inner wall, it will perform a correction to the steering. Finally, a **PID steering control** ensures smooth and precise turns based on this calculation, keeping the robot aligned while following the wall safely.


<img width="661" height="410" alt="Drive Function" src="https://github.com/user-attachments/assets/9a246d13-acf2-4cbe-a386-9e700c59942d" />



  Moreover, the **DriveDegrees function** moves the robot forward in rotation degrees. He robot will keep driving at the given speed until the target degrees are reached, and stops the motor if stop is set to 1.

<img width="753" height="206" alt="DriveDegrees Function" src="https://github.com/user-attachments/assets/2be20ba8-d542-44c5-871f-9f2dcbf409cd" />




**(f) Main program**

This program resets timers and steering, then drives forward until it detects a wall on either side. It determines whether to follow the right or left wall based on sensor readings.

<img width="480" height="366" alt="Determine Direction" src="https://github.com/user-attachments/assets/a4d46f80-6c0e-4bff-97ea-f95532cf990b" />


<img width="1272" height="431" alt="Determine Direction (2)" src="https://github.com/user-attachments/assets/d58c8a4b-1f1b-484f-9ff1-56f77e3fbcd6" />



  When the robot enters the **second section,** it does **not immediately start wall tracking.** Instead, it first drives a certain distance in degrees before activating wall tracking. This is done to **prevent sudden corrections.** If the robot starts tracking the wall when the sensor values are far from the desired distance, it could make a sharp turn and accidentally hit the wall. After driving the initial distance, **wall tracking (trackWall)** is turned on, and the robot begins adjusting its direction to follow the wall smoothly. While tracking, the robot moves at a **controlled speed of 80,** which ensures stable motion and reduces the risk of collisions as it approaches the wall.

<img width="530" height="522" alt="TrackWall" src="https://github.com/user-attachments/assets/30b3bb10-a3b7-4a90-bf23-ce0ba29cfe4a" />

  Then, it loops the same program for **10 times, turning 90°** in the chosen direction in every loops. After completing the 10 loops, the robot enters the **last section.** It updates the target from time to time and drives forward while checking the **Y-coordinate** until it is roughly within the range -1 to 1, which represent that the robot will stop at the **(0,0) position.** Once there, the robot stops all motors and pauses for 2.5 seconds to complete the task.

<img width="794" height="521" alt="Y-coordinate" src="https://github.com/user-attachments/assets/fcaa00d1-e8bf-49af-a77e-82b80ce4a1f8" />



## 3.2 Obstacle Challenge
To complete the **Obstacle Challenge,** our robot utilizes four sensors which is **one Pixy2 Camera, one gyro sensor, two ultrasonic sensors** on both the left and right sides and **one colour sensor.** Since both ultrasonic sensors need to be connected to the same port, we use the **multiplexer** so that the robot can read data from both of the sensors.


<img width="1920" height="1080" alt="Sensors" src="https://github.com/user-attachments/assets/5eea41fc-5749-47a5-9d5e-d648d1c71e56" />



The **Pixy2 Camera** is connected to port 1 and it helps to detect the presence of pillars and magenta parking lot during the round. Next, the **EV3 Gyro Sensor** that connected to port 2 helps to ensures that the robot does the accurate turns and keep the robot’s heading straight during the round. In addition, both of the **EV3 Ultrasonic Sensor** is connected to EV3 Brick port 3 via the multiplexer. They help to detect the presence of the inner and outer wall and prevent the robot from hitting into the wall. Lastly, we utilize the **EV3 Colour Sensor** to identify the coloured line on the map which is the orange and blue line. The identified colour allows the robot to know the direction accurately. For instance, if orange line is scanned first, the direction will be in clockwise direction.

Here is the quick overview about the program. When the robot begins, it first **resets its steering mechanism** to ensure it starts from a centred and accurate position. As the robot drives, a **PID steering control system** is used to maintain stable movement and the correction such as gyro correction and keeping optimum distances from the outer wall. During the round, the **Drive function** continuously combines inputs from pillar detection, wall tracking, and PID correction. The sensors such as Pixy 2 Camera allows the robot **to identify traffic sign accurately** and choose the correct avoidance direction. After completing its last sections in the loop 12, the robot will **reverse to hit the wall** and aligns with the parking area and finally **performing a side parking neatly into the magenta parking zone.**



Diagram below shows the flowchart for **Obstacle Challenge:** 

<img width="1910" height="2349" alt="Obstacle Challenge Flow Chart" src="https://github.com/user-attachments/assets/f9795228-6d92-4b51-a86f-bb991470b5ce" />


**Appendix 3** contains the complete programming code for the **Obstacle Challenge.**

### 3.2.2	Coding explanation

Below is a brief explanation of the key parts of the code used to control the robot during the challenge.

**(a) Initialization and Set Up**

This part is aim to set up the **Pixy2 Camera** and **multiplexer** before running. The **setLampOn** and **setLampOff** function turns the lamp of the sensor on and off while the **getSignature** function allow the **Pixy2Camera** to read the position of the green and red pillars through their XY coordinate shown in the **Pixy Mon V2** apps. The **setMultiplexerMode function** allows the EV3 to connect with both ultrasonic sensors in the same port while the **getMultiplexerValues function** allows the robot to read the distance values from the left and right ultrasonic sensors. 

<img width="769" height="522" alt="Initialization and Set Up" src="https://github.com/user-attachments/assets/eb312e2a-e013-41b1-8dbe-77bb7cf4afda" />



Plus, each sensor such as **EV3 Gyro Sensor, EV3 Color Sensor, EV3 Ultrasonic Sensor** and **Pixy2 Camera** must be set up to their own port before the robot starts. **ReadSensor** continuously updates the **green (Signature 1)** and **red (Signature 2)** pillars positions on the camera views. The **magenta parking lot position (Signature 3)** also updated from time to time. Moreover, the robot also reads the **gyro angle** and **wall distance** in real time so that the robot will not off from its target.

<img width="394" height="361" alt="ReadSensor Function" src="https://github.com/user-attachments/assets/3ed354d4-5c6a-499e-ba67-be7f6ad0e19f" />


The **GyroReset** allows the robot to reset the gyro sensor so that the gyro will measure the angles from zero again. It is like pressing the “reset” button on the **EV3 Gyro Sensor** so that it starts measure the heading from 0 again. This is important because it avoids cumulative errors that might affect the robot.

<img width="631" height="268" alt="GyroReset Function" src="https://github.com/user-attachments/assets/f208217f-3395-4e6f-82b1-abce63c3ae28" />

**(b)	Car Position Coordinate Tracking**

This part helps to **track the robot’s position** by calculating its movement along the **Y-axis.** The robot estimates its position based on two main factors which is the **speed of the drive motor** and **the angle measured by the gyro sensor.** By applying the cosine of the gyro angle, the program determines how much of the robot’s movement contributes to vertical travel, which is the y-axis and the value will be **stored in MapY.** To maintain accuracy, the program continuously recalculates MapY in real time as the robot moves. The updated value is displayed on the LCD screen, allowing users to monitor the robot’s position throughout the run. To avoid unrealistic or drifting values, MapY is also **restricted within a specific range.** When the robot is in a clockwise direction, MapY is allowed to vary between –20 and 40. In contrast, during a counter-clockwise run, the allowed range is shifted to between –40 and 25.

<img width="698" height="479" alt="Car Position Coordinate Tracking" src="https://github.com/user-attachments/assets/cf8624a0-8ddb-4129-adcc-44997ee30bce" />


**(c)	Reset Steering**

The **ResetSteering** helps to reset the steering motor before the robot starts running. It will turn the steering wheel all the way to one side and let the robot know the starting point. This is important because it will allow the robot steering always aligned in middle before it starts to move.

<img width="480" height="286" alt="Reset Steering" src="https://github.com/user-attachments/assets/b1ea82db-215c-4cc3-af99-7d7ea4d29c37" />



**(d)	PID Steering Control**

The **PID Steering function** helps the robot to adjust the steering motor whenever it starts to drift off from the target. This function is crucial in the **Obstacle Challenge** because it allows the robot to maintain in the straight heading after avoiding the pillars. The **P** part fixes most of the error right away, the **I** part makes small adjustments over time and the **D** part make sure that the correction is done smoothly. These three adjustments are added together to get one correct value, which is sent to motor A to turn the steering. This keeps the robot moving smoothly, avoiding zig-zagging, and makes its turns more accurate.

<img width="588" height="402" alt="PID Steering Control" src="https://github.com/user-attachments/assets/95a30cfb-2bf9-4de0-a0f1-0f49bd8a6dd0" />


**(e)	Drive**


The **Drive** function combined four main parts which including the **TrackWall, TrackPillar** and **PID Steering.** In sum, these values help the robot constantly adjust its steering and make sure the robot move smoothly and accurately.

**(i)	TrackWall**

The robot checks its **distances from the walls** within the range of 150mm. If it’s too close to one of the sides, it will steer away. Plus, the robot will **check which wall is closer by comparing the distance values from both sides.** If the left wall is closer, the robot will adjust its steering to follow the left side. If the right wall is closer, it will follow the right side instead, but with a negative steering value to turn in the opposite direction.


<img width="894" height="279" alt="TrackWall" src="https://github.com/user-attachments/assets/a567943c-8f2a-41a8-b908-5882425187c7" />



If **neither wall is detected** within the set range, the robot will not make any wall-following adjustments. This allows it to **continue moving straight** without unnecessary corrections.
 
<img width="900" height="257" alt="TrackWall Adjustments" src="https://github.com/user-attachments/assets/f9c0c335-8a01-42a9-97f8-215267dcd44f" />



**(ii)	TrackPillar**

This part helps to calculate how far each pillar from the **Pixy2 Camera’s view.** It uses the **Pythagorean theorem** to figure out the straight-line distance based on the difference in horizontal (x) and vertical (y) positions.

<img width="841" height="118" alt="Pythagorean Theorem" src="https://github.com/user-attachments/assets/0c5f4df6-d903-4864-8460-d0f9f4e815b3" />



This part helps the robot to check the presence of **red, green pillars** and **magenta** parking lot. If the pillars are near to the robot, the robot will start reacting by showing the LED colours. If the **green pillar** is the closest, it sets **@lastPillar = 1** and lights the **green LED.** Additionally, the y-coordinate (150) allows the robot to know the distance of the pillar from the Pixy2 Camera’s view. However, if the **red pillar** is the closest, it sets **@lastPillar = 2** and light **red LED.** The steering will start to do the adjustment once the red pillars is located at the y-coordinate value (160) from the Pixy2 Camera’s view. If the **magenta parking lot** is near, the **orange LED** lights up. The robot will steer to the **right** if it is moving clockwise, or to the **left** if it is moving counter clockwise to avoid hitting the magenta parking lot.

<img width="876" height="659" alt="TrackPillar" src="https://github.com/user-attachments/assets/2f4d8094-b993-4140-89f3-962b385ad54a" />



When no pillar is nearby, the robot turns off its **LED light** and uses the **ultrasonic sensors** to follow the wall. If it is moving clockwise, it will check the left wall. Conversely, if it is moving counter clockwise, it will check the right wall. If it is too far off its intended direction (relative heading), it will not make any wall adjustments to avoid over-correcting. 

<img width="900" height="219" alt="LED Light OFF" src="https://github.com/user-attachments/assets/4cf79d71-03a2-4cf8-9121-e090d6c74164" />



**(iii)	Steering Error**

The robot’s steering correction is based on a combination of **pillar tracking and wall tracking.** The robot then applies this correction to the **PID steering motor.** At the same time, it powers the **drive motor** which is the Motor D to move forward at **runSpeed.**

<img width="601" height="232" alt="Steering Error" src="https://github.com/user-attachments/assets/fc3cb26a-ad6c-46bc-bd08-47a6b7650a79" />


**(f) Others movement block**

Below shows the others movement block that help the robot to perform better.

**(i)	WaitDegrees**

The **WaitDegrees** function makes the robot to move a certain distance based on the rotation of its drive motor **(Motor D).** The stop=1 means the robot will stops the motor and waits for a 50ms after finishing the movement.

<img width="780" height="313" alt="SteeringDrive" src="https://github.com/user-attachments/assets/99769d74-2a74-4274-9cb9-55f82bda30b7" />




**(ii)	SteeringDrive**

The **SteeringDrive** function makes the robot move forward a certain distance while controlling the steering. Therefore, it will combine the current steering motor position with any additional steering adjustment during both of the challenge rounds. 

 <img width="653" height="257" alt="image" src="https://github.com/user-attachments/assets/de204873-25f9-4150-b020-8e5a967def56" />


**(g) Main program**

When the robot starts, it first decides whether it will move in a **counterclockwise** or **clockwise** direction based on the ultrasonic sensor readings. As shown in the diagram below, if the left wall distance is greater than the right wall distance **(leftWall>rightWall),** the robot will know that it is counterclockwise. However, **if the right wall is greater than left wall (rightWall>leftWall),** the robot will know that it is in clockwise direction.

<img width="760" height="553" alt="Determine Direction" src="https://github.com/user-attachments/assets/80cbedeb-f5fa-469a-8ca6-8505f74db224" />


 
Next, the pillar X value tells the robot where the pillar should appear in the camera’s field of view. By using this value, the robot will avoid the pillar or adjust its path to stay centred when following it. 



 
Next, the pillar X value tells the robot where the pillar should appear in the camera’s field of view. By using this value, the robot will avoid the pillar or adjust its path to stay centred when following it. 

<img width="882" height="499" alt="Pillar Value" src="https://github.com/user-attachments/assets/1668a033-7237-4e17-b719-684dd745f010" />


After exiting the parking lot, the robot will drive forward at a speed of 45 until its colour sensor detects either a blue line or an orange line on the ground. Upon detecting a target line, the robot will immediately play a sound to indicate that the line has been found. 


<img width="681" height="366" alt="Detect Line" src="https://github.com/user-attachments/assets/454198a4-b5d2-49eb-971a-64e37ff503ac" />



During the Obstacle Round, the robot adjusts its steering by correcting any error measured from three sources which include **TrackPillar** and **TrackWall.** The redH and greenH refer to the distances of pillar from the camera view. It allows the robot to know when to do the tracking of the pillars. The steering target is slightly different depending on whether the robot is moving clockwise or counterclockwise so a different adjustment value is applied for each direction. This steering correction process is repeated for 11 loops.

<img width="612" height="361" alt="LoopCount" src="https://github.com/user-attachments/assets/abb3821f-0807-47b4-82c4-98c8de5f4c68" />



The below part of the program ensures the robot does not overturn and end up facing the wrong direction while avoiding a pillar. When the robot avoids a pillar on its left side, which mean it passes a green pillar in a clockwise run or a red pillar in a counterclockwise run. It needs to turn a greater number of degrees. This extra turning ensures it does not accidentally scan the wrong-coloured line, which could cause it to head in the wrong direction.

<img width="460" height="404" alt="Avoid Pillar" src="https://github.com/user-attachments/assets/d274f14d-614c-4c91-a78c-98f7dd0d4b0b" />



The program below indicates the robot had completed 11 loops. If the robot is moving in **clockwise direction (cw=1),** it will continue driving forward as long as its MapY value is less than 4. This means the robot will keep moving until it reaches the target Y-coordinate, ensuring it get into the last section completely before proceed to the reverse movement. Conversely, when the robot is moving in a **counter-clockwise direction (cw= -1),** the target range is different. In this case, the robot will continue driving forward while MapY is still less than –16. Ultimately, this part of the program ensures the robot get into its initial position in the last section to make sure the round is completed.

<img width="331" height="284" alt="Y-coordinate" src="https://github.com/user-attachments/assets/2cbf08ee-e935-46f3-9081-294834b5a57f" />

The below part of the program makes the robot **reverse until it reaches the correct position.** When the robot is **moving clockwise,** it keeps reversing until its y-coordinate becomes **less than –10.** When it is moving **counterclockwise,** it reverses further until the **y-coordinate reaches –25.** This helps the robot gently touch the outer wall so it can straighten itself and follow the wall more easily during the parking phase. After that, the program **turns on wall-following mode,** sets the wall distance to 30 cm, and uses a response value of 0.5 to help the robot correct its steering whenever the distance changes. Finally, the robot continues reversing for 3 seconds to make sure it is fully in position before starting its final parking movement.

<img width="269" height="413" alt="Wall-following Mode" src="https://github.com/user-attachments/assets/d96a850e-3911-4f3e-9efc-bd4fec09deb1" />


Both of the picture below shows the detailed program **during the side parking phase.** The robot will move forward while maintaining a fixed distance from the parking lot which is **260 mm** for both directions. As it moves, it continuously checks this distance. If the distance goes out of range, the robot will **adjust its steering to bring it back to the correct value.** Once it passes the first magenta parking lot, the robot will reverse into the parking space and ensure it is parked parallel to the parking lot.


 	 
<img width="792" height="317" alt="Parking" src="https://github.com/user-attachments/assets/d2b9366d-c206-4b64-87c5-a0fdfa6feb99" />

 
The flow diagram below illustrates the detailed process of side parking.
 
<img width="1920" height="1080" alt="Process of Parking" src="https://github.com/user-attachments/assets/1eb1c139-ce7f-4248-8a15-e7bf0eee0641" />

# 4.0 Engineering Factors
This section showcases our **custom-designed and third-party open-source parts** along with detailed explanations of all the components installed in the car. 

At first, our autonomous self-driving car is **primarily built using the LEGO Mindstorms Education EV3 Core Set 45544.** However, we encountered several limitations while preparing for both the Open and Obstacle Challenges. For example, our design required more sensor ports than the EV3 brick could support, the **Pixy2 Camera was unstable** due to weak mounting, and we **lacked a suitable camera system** to accurately detect the pillars and the magenta parking lot. To overcome these challenges and enhance our robot’s performance, we incorporated **third-party components** into the design. The diagram below illustrates the additional components we used and how they helped overcome these issues.
 

**(i)	EV3 Sensor Multiplexer**

We added an EV3 Sensor Multiplexer so our robot can use five sensors at once. There are two ultrasonic sensors connected to the multiplexer with different channel. With all five working together, the robot can move more accurately and handle Obstacles Challenge better.

<img width="1920" height="1080" alt="EV3 Sensor Multiplexer" src="https://github.com/user-attachments/assets/6a33c235-dacc-49c6-ae42-a85fce2abceb" />



**(ii)	3D Printed Part**

We created a 3D-printed casing for the chassis, steering and camera bracket to improve the robot’s overall performance. 

<img width="1920" height="1080" alt="3D Printed Part" src="https://github.com/user-attachments/assets/d07153e4-0b69-4c32-b673-41a6fbfe94fb" />



**(iii)	Pixy2 Camera**

We use the Pixy2 Camera because it can quickly and accurately detect objects while the robot is moving. In our design, the Pixy2 Camera is mainly used to scan and track the magenta parking lot, green and red pillars, which helps the robot recognize them in time and make the right navigation decisions during the Open and Obstacle Challenges.	. 
 
<img width="873" height="315" alt="Pixy2 Camera" src="https://github.com/user-attachments/assets/76923908-39c1-461f-9ac5-15c529948168" />


# 5.0 Improvements and Enhancements
In this section, we explain the **problems** we faced while building our self-driving car and the different **methods** we used to solve them. By studying each problem carefully, we made changes that improved the car performances. The improvements towards the robot can be categorized into two main parts which is the **construction** and **programming parts.**

## 5.1 Robot construction

We improved the construction of robot from time to time whenever we encountered challenges. Below are some of the improvements we implemented.

**(i)	Replace the front steering wheel with a smaller size wheel**

Initially, we are using the **LEGO tyre 44771** for the front wheel but then we switched to the smaller tyre from Spike Essential Set which is known as the **Medium Azure Hard Rubber Tyre.** The reduced size improved the car’s maneuverability, making it easier to turn and park in tight spaces. Moreover, the steering’s sensitivity is better when avoiding pillars.

<img width="1920" height="1080" alt="Steering Wheel" src="https://github.com/user-attachments/assets/7fda0ca7-bb76-41e3-87b6-f38f3ff1f7cc" />



**(ii) Implementing a multiplexer to solve the limited EV3 ports issue**

We also encountered an issue with the **limited number of EV3 ports.** During the **Obstacle Challenge,** multiple sensors were required at the same time, which quickly used up all available ports. To overcome this, we used **a multiplexer,** which allowed us to **expand the number of connections.** Both ultrasonic sensors were connected to the multiplexer, freeing up the built-in EV3 ports for other essential sensors.

<img width="1920" height="1080" alt="Multiplexer" src="https://github.com/user-attachments/assets/9510c990-b1c7-4e08-984e-801751d1b78f" />


**(iii) Pixy2 Camera Position Adjustment**

Initially, the camera sometimes **detected the wrong objects** and treated them as pillars. This happened because the camera angle was too wide. So, we adjusted the Pixy2 camera angle from **75° to 65°**. With the smaller angle, the camera focuses better on the actual pillars and **avoids capturing unnecessary objects.** This helps the robot steer correctly and reduces mistakes during the Obstacle Challenge.

<img width="1920" height="1080" alt="Pixy2 Camera Position Adjustment" src="https://github.com/user-attachments/assets/797b0bd3-025c-4d5d-b04b-95162579759c" />




## 5.2 Robot Programming

We refined the programming of our robot from time to time whenever we faced issues, making adjustments to improve its performance.

**(i)	XY-Coordinate Position Tracking**

Previously, our robot relied on degree measurements to enter the final section of the challenge. However, during testing, we realised that this method was unreliable because the wall length in the Open Challenge was not always the same. To improve this, we introduced a coordinate-based positioning system. Instead of depending on motor degrees, the robot now calculates its X and Y positions using its gyro angle and wheel speed. This allows the robot to know where it is and move into the final section more accurately, even if the wall layout changes. After applying this improvement, the robot enters the last section consistently and with much better precision.

<img width="732" height="325" alt="XY-Coordinate Position Tracking" src="https://github.com/user-attachments/assets/4521862c-d1b8-4796-b5e4-19dec55eb55b" />

  
**(ii)	Resetting the gyro**

When we tested our EV3 robot, we noticed the gyro sensor sometimes drifted. This means that even when the robot was not turning, the angle reading slowly changed. At first, we tried fixing it by adding a software reset in our program. The reset switched the sensor into the correct mode, sent a command to set the angle back to zero, and waited until it was ready. This worked most of the time, especially when we reset it just before the robot started moving.

<img width="812" height="305" alt="GyroReset" src="https://github.com/user-attachments/assets/62b4d82c-9e24-4e2a-b897-ab558c99af7a" />


However, we found that the gyro could still drift during the run, even after the software reset. Things like vibration, motor movement, and small calculation errors could still affect the reading. Hence, we decided that a hard reset might work better. A hard reset clears the sensor’s memory more deeply than a software reset, giving a cleaner and more stable reading at the start.

<img width="770" height="666" alt="Unplugging Port" src="https://github.com/user-attachments/assets/fe586ae9-0bc6-4ae9-9c32-23b8e264c217" />



**(iii)	Ensuring continuous operation of ultrasonic sensor**

The ultrasonic sensor has an issue where it may **turn off unexpectedly during operation** without any warning. To address this, we've developed a program that automatically **sets the robot's motor speed to zero whenever the ultrasonic sensor detects a value of zero.** This precaution effectively stops the robot's movement until the sensor resumes normal operation, reducing any risks associated with the sensor failure. Once the ultrasonic sensor begins detecting values again, the robot will r**eturn to its normal speed,** ensuring smooth and uninterrupted movement.

<img width="691" height="133" alt="Continuous Operation of Ultrasonic Sensor" src="https://github.com/user-attachments/assets/ba252081-a3ef-421c-8519-f371fb416109" />


 
**(iv)	Adding signal light to EV3 Brick**

At first, we did not connect the Pixy camera with the EV3 brick’s LED light. This made it **harder** to know when the robot had spotted a pillar. During testing, we had to **guess** whether the robot was reacting at the right time.

To make this easier for competition, we set the **LED to change colour when the robot sees a pillar.** By looking at the LED and the robot’s position on the map, we can **quickly** confirm if it is reacting **too early or too late.** We also thought about adding sound alerts, but in a crowded and noisy place, it would be **difficult to hear** them. That’s why using lights is a better choice to overcome the problems.

  
<img width="971" height="838" alt="Signal Light" src="https://github.com/user-attachments/assets/71d4d4e4-2b4f-4e92-a6b3-8afd408744bd" />


**(v)	PID Steering**

Before this, we didn’t use **PID steering** in our robot’s program. From our observation, the steering corrections were not precise. The robot sometimes drifted off track or turned too much, which made it slower and less accurate.

To solve this, we added **PID steering.** This allows the robot to constantly adjust its steering to follow the target path more accurately. After adding PID, the robot **turns smoothly** and stays on track much better. This greatly improved our performance in both of the challenges. The video in the QR code clearly shows the difference when PID steering is applied.

Programming of the PID steering system

<img width="738" height="469" alt="PID Steering" src="https://github.com/user-attachments/assets/fd699bc2-9466-4e43-80b1-1a4963d959a0" />

PID Steering System Demo
https://youtu.be/QbyQ7LRgAdg 

<img width="472" height="467" alt="PID Steering (Video)" src="https://github.com/user-attachments/assets/a4351a97-15de-46dc-95ab-69a030625d64" />




# Credits

We extend our sincere appreciation to our key supporters. Special thanks to LEGO Education for their generous provision of high-quality EV3 and SPIKE Essential sets. We are also grateful to Bambu Lab, whose advanced 3D printing technology was instrumental in the development of our custom components.


# Appendix 1. The Building Instruction of the Self-Driving Car

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/fa4d5e48-d6d7-4192-b123-f4ff5f3e92a4" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/2cb66d7f-481c-44f1-87aa-6131aceb14f6" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/6142c415-f906-4126-b7d7-1e2f919b36ca" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/79fefd3d-4241-4745-95ce-2d4c623714d6" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/df8c78ff-a93c-4875-9532-a603f6ab59bb" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/5d816a8a-236d-46f0-be15-6cfae7c03e0e" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/fa48b079-17bf-4871-afbe-fc8a5d91e8d8" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/e5159f07-de6a-44a2-89e2-7751671f4c35" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/de8f4d11-37be-4400-8f2c-77fdebdb7606" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/bc19e164-19bf-4136-8b83-bf979ad556da" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/4325b0e1-d22d-4954-8ab8-9740615a1ccf" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/be0ed891-7e97-4664-a180-2538f84cb463" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/c80f4004-a160-4e4a-b422-3a81ab771eea" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/8c7608e6-2fb2-4912-b985-c2ab2c717c0d" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/1c3b51df-69ab-4716-931c-29a2bebf5b38" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/4b035f92-d35a-4945-9b90-194a4c9c9255" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/4721abd7-fd24-434c-9caa-b12085b32fbf" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/bdcdb292-7a40-409f-8688-d73eafb8d941" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/73d38d35-567e-493a-9dd8-2eb2ed06cade" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/24d1a3fb-5182-42d1-a1cc-a09292b86b0b" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/57d6f0a4-66bc-4c39-b583-c8e997205afa" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/3cd366e0-edfe-4ad4-bfcf-e8b69c7e723f" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/d8f9897a-fcae-48f2-aed8-94dc01855714" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/e8281551-3cc0-453c-a0ca-0d40618cfbdd" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/8dd2dea5-e7c5-4300-9143-756abe8c5da2" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/57f7b8a8-dfd2-4622-b47c-a57b73dabc2e" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/2d2feb18-92a0-455d-b206-a440b373c3be" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/3322164f-3078-4866-bac0-1b05935e434c" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/9edfbc98-9d23-4f3d-8da0-b623e8397605" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/32463d49-879f-44fa-bb98-8baa7e2980eb" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/ffd96a48-beb2-4bd4-867e-750f70e1ce14" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/fbcdfe76-22bf-4af4-a752-e53d5762864d" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/48452d63-6f9a-4b0b-8f7f-8f165f2b06c7" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/6d2cfa76-6cb4-4989-8443-950d54f0e3b3" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/43ab49b0-221d-4990-989d-43532050a305" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/fbee01ce-1ef4-4262-a418-95d1269c0049" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/7de38716-f444-4132-94ab-5c5ddae82b57" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/6b2446a6-6596-4085-bf05-a420d9a9ebdb" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/3f58f54b-f337-4f24-8613-243d08055faa" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/14d2fc1e-da42-4b47-b7f2-5f1f45a162ff" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/da661cf5-acb4-413a-8209-e1b6123d3b93" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/966dfbe7-b95d-4dae-8163-4268fca5ff54" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/7cb40d31-bcae-4575-8224-abe6654b3847" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/eec91ed5-33ae-4cdf-9259-1ff1071491c9" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/70b5f977-6cf1-429f-bd09-b3c21183235a" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/f61f2264-24b2-4e65-a018-bcba85a13669" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/ccc7562f-a020-4802-b598-354cc2c29224" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/946504e0-08b0-4bbb-8607-6a1692fcc7bf" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/00f3279a-9f35-4c92-9519-6e1314a2aa6c" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/0049e761-f0ea-4376-a5b8-a4b3e9d288bd" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/00fd7cb4-cb86-4de1-a1d5-2317cf12eddb" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/8d262737-b364-4496-a0f9-b7619db48348" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/039ada3f-ebc0-483c-9db7-2dd2e0879b25" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/98b36196-60de-4096-a2ca-46b3e91fe682" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/ef854370-7b57-43f6-b726-632ef8355661" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/ccfa7685-16ff-49f5-84cf-d23192920bb7" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/d82967e1-0f92-4c8e-b99f-f1f951571136" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/add56105-77db-4f58-b8ae-8a84ccb3bbc0" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/e1ac833e-3f73-4906-8914-4be019c58c88" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/31a9c81d-c3d5-475b-a84c-d899e874cfbc" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/af4ff8d1-de5f-4279-a3fe-78fa1b1a6bea" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/4f36fe09-a767-4e4e-8a5b-02368cd68d26" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/263dfc17-f495-4cf7-91c5-402675f72d09" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/0c98d8ac-f73c-4e23-9462-3070d6aae960" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/c9d47171-62df-4e9a-b255-3a3a9b770cf0" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/fd5e45c8-a6fa-4a6e-8002-2e3ff0f39090" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/d544c54d-eaff-4294-b0d4-bf93a0b09526" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/d4757ea5-64dc-433b-9a94-11f62935d24b" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/0346024a-8b81-495e-b27c-12822a348600" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/9a92d21a-57ab-4c3b-8f22-6da14cf3377b" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/0574f49e-e626-4d93-b987-59d0b0037570" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/5f08c824-aa5f-49c8-817e-887d4bbf110b" />

<img width="940" height="1327" alt="image" src="https://github.com/user-attachments/assets/2f439e36-4daf-47cc-81ed-66f72e1a589e" />


# Appendix 2. Open Challenge Programming

<img width="940" height="681" alt="image" src="https://github.com/user-attachments/assets/5e21d77b-505c-43a5-b24f-ea253caae83f" />

<img width="940" height="534" alt="image" src="https://github.com/user-attachments/assets/0df60be3-0a41-41c0-9c62-b578017777b4" />

<img width="940" height="539" alt="image" src="https://github.com/user-attachments/assets/fbb78f3e-2c68-4234-8b44-9fe31aa79aa7" />

<img width="940" height="674" alt="image" src="https://github.com/user-attachments/assets/1963692f-c910-4f56-b94a-460b3521fc92" />

<img width="940" height="578" alt="image" src="https://github.com/user-attachments/assets/404cedab-79e7-46b8-a80b-7608f1f61bcb" />

<img width="940" height="430" alt="image" src="https://github.com/user-attachments/assets/d4f10bfb-84da-415d-9d98-da7c134904cd" />

<img width="940" height="612" alt="image" src="https://github.com/user-attachments/assets/40acad00-d192-45c2-995e-7b3d5357d1a4" />


# Appendix 3. Obstacle Challenge Programming

<img width="940" height="603" alt="image" src="https://github.com/user-attachments/assets/3bec1c79-07d2-43a5-9c29-477ba2229c3d" />

<img width="940" height="531" alt="image" src="https://github.com/user-attachments/assets/0edba2d5-5d5c-4b01-9f7f-e0d0d2517336" />

<img width="940" height="485" alt="image" src="https://github.com/user-attachments/assets/3cd58a76-2054-443c-8edf-b30ae7315106" />

<img width="940" height="555" alt="image" src="https://github.com/user-attachments/assets/735942d7-e9a5-4f72-80bc-f56e4f92902f" />

<img width="940" height="561" alt="image" src="https://github.com/user-attachments/assets/2bed3e17-0a75-4144-a935-f2fe30be0c7e" />

<img width="940" height="535" alt="image" src="https://github.com/user-attachments/assets/037d7a8c-3fad-41d1-b53f-1a70b630381b" />

<img width="940" height="521" alt="image" src="https://github.com/user-attachments/assets/771f719f-18b2-42ca-8b51-b4c05a520f39" />

<img width="940" height="623" alt="image" src="https://github.com/user-attachments/assets/8e25456d-d567-401e-b02b-361a1d589812" />

<img width="940" height="459" alt="image" src="https://github.com/user-attachments/assets/d4a4362a-d955-4c8c-b344-34291f1ac6ce" />

<img width="940" height="483" alt="image" src="https://github.com/user-attachments/assets/e9e165a8-4508-4a7f-a550-513669f9bf69" />

<img width="940" height="537" alt="image" src="https://github.com/user-attachments/assets/54ee7551-ce55-4b74-887a-c8414dfc4636" />

<img width="940" height="616" alt="image" src="https://github.com/user-attachments/assets/a71d265f-8f3a-4181-80db-ba8adc659f52" />

<img width="940" height="637" alt="image" src="https://github.com/user-attachments/assets/4f50cabb-30bc-4f30-bce7-e8ddf5f7ee1a" />

<img width="940" height="599" alt="image" src="https://github.com/user-attachments/assets/d3755269-0e68-4658-8332-1d911b42d32a" />

<img width="940" height="707" alt="image" src="https://github.com/user-attachments/assets/3561e90c-ff29-4e2d-b0a7-69b96094e29e" />

<img width="940" height="645" alt="image" src="https://github.com/user-attachments/assets/51d55b24-98ed-41f7-b466-b39f73219e40" />

