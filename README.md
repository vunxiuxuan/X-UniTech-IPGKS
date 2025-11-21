
# Content (GitHub)
**schemes** This folder contains one or several schematic diagrams in the form of JPEG, PNG, or PDF of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they connect. This folder also included the schematic diagram of the robot for both open and obstacle challenge.

**src** This folder contains all the programming flowcharts and all programming used to participate in the WRO 2025 Future Engineers Category.

**t-photos** This folder contains photos of the team participating in the WRO 2025 Future Engineers Category.

**v-photos** This folder contains photos of the vehicle from all sides (top view, bottom view, front view, back view and side views)

**video** This folder contains video.md file that demonstrates how the robot functions to solve both challenges.

**models** This folder contains the robot building insturction and the 3D printed part building instruction that installed on the vehicle. The file is presented in .lxf, .ldr and .ldr format.

**other** This folder contains other files which can be used to understand how to prepare the vehicle for the competition.

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
  - [2.2 Sensors](#22-sensors)
  - [2.3 Build Of Materials (BOM)](#23-build-of-materials-bom)
  - [2.4 Wiring diagram](#24-wiring-diagram)

- [3.0 Obstacle Management](#30-obstacle-management)
  - [3.1 Open Challenge](#31-open-challenge)
  - [3.2 Obstacle Challenge](#32-obstacle-challenge)

- [4.0 Engineering Factors](#40-engineering-factors)
  
- [5.0 Improvement and Enhancement](#50-improvement-and-enhancement)
  - [5.1 Robot Construction](#51-robot-construction)
  - [5.2 Robot Programming](#52-robot-programming)

- [Credits](#credits)

- [Appendix 1. The Building Instruction of the Self-Driving Car](#appendix-1-the-building-instruction-of-the-self-driving-car)
- [Appendix 2. Open Challenge Programming](#appendix-2-open-challenge-programming)
- [Appendix 3. Obstacle Challenge Programming](#appendix-3-obstacle-challenge-programming)

# Introduction
This engineering documentation details comprehensive aspects of the car’s mobility management, power and sensor systems, obstacle detection and avoidance, construction design, integration of third-party sensors, and the improvements that were made throughout our preparation for the World Robot Olympiad (WRO) International Final in Singapore 2025 under the Future Engineers Category.


# X-UniTech Team, Malaysia
X-UniTech is a team from Malaysia consisting of three-member engineering team specializing in the development of autonomous vehicles. Our team is responsible for the end-to-end design, construction, and integration of the vehicle's mechanical and electronic systems to ensure optimal performance. Let’s meet our members:

**Vun Xiu Xuan, Alvin Kong Wei Ee, and Grace Tan Hong Hui.**

<img width="1020" height="764" alt="Team Photo" src="https://github.com/user-attachments/assets/9270f1dd-48bb-4caf-93c4-008a8048cd62" />

# Performance video
This video demonstrates our autonomous vehicle's design and its operational performance in both the Open Challenge and the Obstacle Challenge. Kindly scan the QR code below or access the link to watch the video for both challenges. https://youtu.be/pi9NsIusMks

<img width="250" height="250" alt="Performance Video (YouTube)" src="https://github.com/user-attachments/assets/e27dbd22-1fb4-488e-ad44-9704f637ad07" />

<img width="250" height="250" alt="Performance Video (Google Drive)" src="https://github.com/user-attachments/assets/9b49bde9-0131-4191-98f3-3d17b8937ec4" />

# 1.0 Mobility Management
This section details the mechanical design and propulsion system of our autonomous vehicle. It covers the chassis construction, component layout, and the integration of the motors. Additionally, it introduces the fundamental engineering principles of speed, torque, and power that govern the vehicle's performance.


## 1.1 Design of the self-driving car
The autonomous self-driving car chassis and mechanical structure are built using the Lego 45544 Mindstorms EV3 Education Set and various third-party sensors such as Pixy2 Camera and EV3 Multiplexer.

<img width="1920" height="1080" alt="Lego 45544 Mindstorms EV3 Education Set" src="https://github.com/user-attachments/assets/e4e4a845-6d69-4b65-a35b-6dd13c652df5" />


The figures below show the autonomous vehicle we designed and constructed.  


Top view	

<img width="1920" height="1080" alt="Robot (Top View)" src="https://github.com/user-attachments/assets/bc4a3e61-c65b-4ee0-93c7-85319cfcf775" />


Bottom view 

<img width="1920" height="1080" alt="Robot (Bottom View)" src="https://github.com/user-attachments/assets/c8b20f0e-9017-4c2f-8956-5c429a31611a" />


Front view	

<img width="1920" height="1080" alt="Robot (Front View)" src="https://github.com/user-attachments/assets/a4670633-ccd4-480d-9ede-2802662e1a39" />


Back view 

<img width="1920" height="1080" alt="Robot (Back View)" src="https://github.com/user-attachments/assets/fd65f990-3e34-4027-a636-42cb5d000160" />


Left side view	

<img width="1920" height="1080" alt="Robot (Left Side View)" src="https://github.com/user-attachments/assets/80207a5e-1eb6-45c8-8068-612a19bd2fc0" />


Right side view 

<img width="1920" height="1080" alt="Robot (Right Side View)" src="https://github.com/user-attachments/assets/a5b661ce-f8d7-4787-88ac-4b59aa907e47" />



## 1.2 Chassis of the self-driving car
The self-driving car chassis is designed to provide structural support and maintain stability, especially during high-speed maneuvers like sharp turns and rapid acceleration.


**(i) Selection of tyre**

For the front steering axle, we selected the Medium Azure Hard Tyre from the Spike Essential set because of its hard rubber compound that minimizes bouncing, allowing the vehicle to track in a straight line more reliably compared to softer tyres. The tyre's smaller diameter enables smoother and more precise steering corrections.

<img width="1920" height="1080" alt="Medium Azure Hard Tyres" src="https://github.com/user-attachments/assets/5f9d309f-d5bc-4d81-9f06-f58820d1f58c" />



The rear axle is fitted with LEGO MINDSTORMS EV3 tyres (62.4 x 20 mm) on 43.2 mm rims. These tyres were selected for the excellent traction their tread pattern provides on typical competition surfaces, such as floors and mats. This high-grip design prevents wheel slippage during rapid acceleration and high-speed cornering. 

<img width="1920" height="1080" alt="Lego Mindstorms EV3 Tyres" src="https://github.com/user-attachments/assets/b47b9379-f939-4589-8fa2-3fb2f7b2d223" />



**(ii) Implementation of motor and its engineering principle**

Our self-driving car propulsion system consists of two EV3 Medium Motors mounted in a compact, orthogonal arrangement (one horizontal, one vertical). This design offers several key advantages: it optimizes internal space, simplifies the gear train assembly, and contributes to a low center of gravity. A low center of gravity is crucial for maintaining stability during the high-speed maneuvers required in the Open Challenge. 

<img width="1920" height="1080" alt="EV3 Medium Motors" src="https://github.com/user-attachments/assets/82c9303f-119b-4e4c-b1ef-d426487d7c21" />


The diagram below illustrates the specifications and features of the EV3 Medium Motor.

<img width="914" height="559" alt="Specifications of EV3 Medium Motor" src="https://github.com/user-attachments/assets/5dbc4ca2-edca-4869-88de-54c19f1756f7" />


The vehicle's steering mechanism is controlled by an EV3 Medium Motor, selected for its high responsiveness and precision. With a running torque of 8 Ncm and a stall torque of 15 Ncm, the motor provides ample force for steering control. Furthermore, its rotational speed of 260 rpm allows quick rotations, making it well-suited for fine adjustments when avoiding traffic signs. 

 **(iii) Implementation of differential gear**
 
A differential gear is integrated into the drive axle, allowing the left and right wheels to rotate at different speeds. This mechanism is essential for executing smooth, controlled turns, as it prevents wheel binding and improves stability. This is particularly critical when navigating the tight corners found in the Open Challenge. Not only that, our robot also incorporates a step-up gear ratio. This setup makes the wheels spin 1.29 times faster than the motor, increasing the speed from 260 RPM at the motor to about 335 RPM at the wheels. This helps the robot to move faster while at the same time maintaining stability during tight turns.

<img width="1920" height="1080" alt="Differential Gear" src="https://github.com/user-attachments/assets/1c7cc38c-aca0-4bae-8c5e-5b6c5fcd4ea0" />



**(iv) Engineering principle of steering**

The steering system is designed using Ackermann steering geometry. 

<img width="1920" height="1080" alt="Ackermann Steering Geometry" src="https://github.com/user-attachments/assets/95865c69-4f91-40b5-b555-ee7da422e191" />



This principle turns the inner front wheel at a sharper angle than the outer wheel, allowing both to follow ideal concentric turning circles. By minimizing lateral tire scrub, this geometry significantly reduces friction and wear. The primary benefits include enhanced cornering stability, improved traction, and the ability to execute sharp turns with greater precision.


## 1.3 Building of the self-driving car
The building instruction for the self-driving car and the video of showcasing the 3D printing process of its parts can be accessed via the QR Code and link below. 



Building Instruction of Self-Driving Car (PDF format)

<img width="250" height="250" alt="Building Instruction of Self-Driving Car (PDF Format)" src="https://github.com/user-attachments/assets/1248dd7f-9f1d-45a1-96fb-e42d79cac07e" />





3D Printing Process Video

<img width="250" height="250" alt="3D Printing Process Video" src="https://github.com/user-attachments/assets/35378bb6-5235-4c56-966c-2b47691c22bf" />













