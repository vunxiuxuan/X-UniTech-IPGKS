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


## 3.2 Obstacle Challenge
To complete the **Obstacle Challenge,** our robot utilizes four sensors which is **one Pixy2 Camera, one gyro sensor, two ultrasonic sensors** on both the left and right sides and **one colour sensor.** Since both ultrasonic sensors need to be connected to the same port, we use the **multiplexer** so that the robot can read data from both of the sensors.


<img width="1920" height="1080" alt="Sensors" src="https://github.com/user-attachments/assets/5eea41fc-5749-47a5-9d5e-d648d1c71e56" />



The **Pixy2 Camera** is connected to port 1 and it helps to detect the presence of pillars and magenta parking lot during the round. Next, the **EV3 Gyro Sensor** that connected to port 2 helps to ensures that the robot does the accurate turns and keep the robot’s heading straight during the round. In addition, both of the **EV3 Ultrasonic Sensor** is connected to EV3 Brick port 3 via the multiplexer. They help to detect the presence of the inner and outer wall and prevent the robot from hitting into the wall. Lastly, we utilize the **EV3 Colour Sensor** to identify the coloured line on the map which is the orange and blue line. The identified colour allows the robot to know the direction accurately. For instance, if orange line is scanned first, the direction will be in clockwise direction.

Here is the quick overview about the program. When the robot begins, it first **resets its steering mechanism** to ensure it starts from a centred and accurate position. As the robot drives, a **PID steering control system** is used to maintain stable movement and the correction such as gyro correction and keeping optimum distances from the outer wall. During the round, the **Drive function** continuously combines inputs from pillar detection, wall tracking, and PID correction. The sensors such as Pixy 2 Camera allows the robot **to identify traffic sign accurately** and choose the correct avoidance direction. After completing its last sections in the loop 12, the robot will **reverse to hit the wall** and aligns with the parking area and finally **performing a side parking neatly into the magenta parking zone.**



Diagram below shows the flowchart for **Obstacle Challenge:** 

<img width="1910" height="2349" alt="Obstacle Challenge Flow Chart" src="https://github.com/user-attachments/assets/f9795228-6d92-4b51-a86f-bb991470b5ce" />


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


## 5.2 Robot Programming

We refined the programming of our robot from time to time whenever we faced issues, making adjustments to improve its performance.

**(i)	Adding signal light to EV3 Brick**

At first, we did not connect the Pixy camera with the EV3 brick’s LED light. This made it **harder** to know when the robot had spotted a pillar. During testing, we had to **guess** whether the robot was reacting at the right time.

To make this easier for competition, we set the **LED to change colour when the robot sees a pillar.** By looking at the LED and the robot’s position on the map, we can **quickly** confirm if it is reacting **too early or too late.** We also thought about adding sound alerts, but in a crowded and noisy place, it would be **difficult to hear** them. That’s why using lights is a better choice to overcome the problems.

  
<img width="971" height="838" alt="Signal Light" src="https://github.com/user-attachments/assets/71d4d4e4-2b4f-4e92-a6b3-8afd408744bd" />




# Credits

We extend our sincere appreciation to our key supporters. Special thanks to LEGO Education for their generous provision of high-quality EV3 and SPIKE Essential sets. We are also grateful to Bambu Lab, whose advanced 3D printing technology was instrumental in the development of our custom components.
