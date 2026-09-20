# Smart-Wheelchair-Main-Control-Board-PCB
The Main Board is the central hardware routing and power management hub for the Smart Wheelchair System. Built around the ESP32-S3-DevKit, this custom-designed printed circuit board (PCB) integrates power distribution, signal processing and multi-sensor navigation into a single unified architecture.

**Overview**

The Main Board serves as the central hardware routing and power management hub for the Smart Wheelchair System. Designed around the ESP32-S3-DevKitC-1-N32R16V platform, this custom PCB integrates multi-directional ultrasonic obstacle avoidance, inertial navigation, analog joystick control, caregiver override, voice processing, GPS telemetry and dual high-power motor driver interfaces onto a single board. 

**Technical Specifications**

- Processing & System Control
•	MCU Socket: Dual 22-pin header sockets (P1, P2) hosting the ESP32-S3 controller. 
•	User Feedback: Onboard status LEDs (DS1–DS3) and a transistor-driven piezoelectric buzzer (LS1, Q1) for mode indication and obstacle proximity alerts. 

- Dual Power Supply Network
•	Power Input: Primary 12V DC input (12V_NET) via a heavy-duty screw terminal (J1). 
•	5V Logic Rail: Powered by an LM2596S-5.0 buck regulator (U1) with filtering inductors and capacitors. 
•	3.3V Sensor Rail: Powered by an LM2596S-3.3 buck regulator (U2) supplying noise-sensitive microelectronics.

- Sensor & Telemetry Integration
•	Obstacle Avoidance: 4 dedicated JST connectors (J2–J5) for a multi-directional ultrasonic sensor array. 
•	IMU Navigation: 8-pin interface (P3) routed to I2C and interrupt lines for MPU-6050 orientation tracking. 
•	Wireless & Voice Routing: Headers for GPS (P6) and Voice Recognition (P7) modules via dedicated UART channels. 
•	Auxiliary Port: 6-pin expansion header (P5) for extra sensors. 

- Drive & Control Interfaces
•	Joystick Control: 5-pin JST port (J6) for dual-axis analog input (JOY_X, JOY_Y) and mode selection. 
•	Caregiver Override: 4-pin interface (P4) reserved for remote override signal receivers. 
•	Motor Actuation: Two 8-pin high-current connectors (J7, J8) routing RPWM, LPWM and enable signals to IBT-2 (BTS7960) motor drivers.

**Connector Quick Reference**

J1 Screw Terminal	- 12V Power Input 

P1 / P2 Female Headers -	ESP32-S3 Board Socket 

P3	8-Pin Header - MPU-6050 IMU Interface 

P4	4-Pin Header	- Caregiver Remote Interface 

P6 / P7	4-Pin Headers -	GPS & Voice UART Ports 

J2 – J5	B4B-XH JST -	Ultrasonic Sensor Array 

J6	B5B-XH JST -	Analog Joystick Control 

J7 / J8	B8B-XH JST -	Dual IBT-2 Motor Driver Outputs

![Project Screenshot](https://github.com/rsmpdo/Smart-Wheelchair-Main-Control-Board-PCB/blob/main/Images/01.png?raw=true)

More project Details : Smart Wheelchair with Voice Control at https://www.linkedin.com/in/shashika-madhusankha-99aab9311/details/projects/

