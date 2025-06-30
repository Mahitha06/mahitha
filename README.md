# Rain Rain Go Away 
## Automated Rain Detection and Wiper Control System:
 ### Project Description:
This project aims to design an automated rain detection and wiper control mechanism. The system detects rain using a sensor and activates a wiper that oscillates from 0 to 180 degrees while displaying four discrete, controllable speed levels.<br/>
The features of thsi project are : <br/>
#### Rain Detection:
Uses an analog sensor to detect rainfall intensity.
#### Speed Control: 
Implements four discrete wiper speed levels based on rain intensity.
#### PWM Control: 
Generates Pulse Width Modulation (PWM) signals for speed variation.
#### Arduino Integration:
Uses an Arduino UNO to process signals and control the servo motor.
#### Servo Motor Indicator: 
Displays the selected speed using a servo needle mechanism.
### System Overview :
#### 1️⃣ Comparator Network
Converts the sensor's analog output into discrete digital signals.<br/>
Uses Op-amp based voltage dividers to define reference levels.<br/>
Outputs digital signals (A, B, C, D) that correspond to different rain intensities.<br/>
#### 2️⃣ Digital-to-Analog Converter (DAC)
Uses a non-inverting summing amplifier to generate different DC voltage levels.<br/>
These voltages are used for PWM generation.<br/>
#### 3️⃣ PWM Generation
Uses a triangle wave generator and a comparator.<br/>
PWM duty cycle increases with rain intensity, controlling motor speed.<br/>
#### 4️⃣ Motor Driver & Wiper Movement
A motor driver circuit with limit switches enables smooth oscillation (0-180 degrees).<br/>
PWM controls speed, while switches toggle motor direction.<br/>
#### 5️⃣ Servo Motor for Speed Indication
A servo motor-based needle visually represents speed levels.<br/>
### Hardware Components:
-Rain Sensor<br/>
-Op-Amps (Comparator Network)<br/>
-Arduino UNO<br/>
-Motor Driver (L298N or similar)<br/>
-Servo Motor<br/>
-Limit Switches<br/>
