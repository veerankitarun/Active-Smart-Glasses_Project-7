                                                        Active-Smart-Glasses 


## About HC-SR04 Module

Ultrasonic Sensor sends out a high-frequency sound pulse and then times how long it takes for the echo of the sound to reflect back. The sensor has 2 openings on its front. One opening transmits ultrasonic waves, the other receives them. 

  ## FEATURES OF HC-SR04

- Power Supply :+5V DC
- Quiescent Current : <2mA
- Working Currnt: 15mA
- Effectual Angle: <15°
- Ranging Distance : 2cm – 400 cm/1″ – 13ft
- Resolution : 0.3 cm
- Measuring Angle: 30 degree
- Trigger Input Pulse width: 10uS
- Dimension: 45mm x 20mm x 15mm
  





![hc-sr04](https://user-images.githubusercontent.com/61703896/174465783-dffa5075-631b-4154-bf37-8ec4badef677.png)

## TIMING DIAGRAM
![timing-diagram-1-768x521](https://user-images.githubusercontent.com/61703896/174466212-869224fb-791c-4a93-acdd-9b1e9ab4d56f.jpg)

Trig of SR04 must receive a pulse of high (5V) for at least 10us, this will initiate the sensor will transmit out 8 cycle of ultrasonic burst at 40kHz and wait for the reflected ultrasonic burst. When the sensor detected ultrasonic from receiver, it will set the Echo pin to high (5V) and delay for a period (width) which proportion to distance. To obtain the distance, measure the width (Ton) of Echo pin

Time = Width of Echo pulse, in us (micro second)

      Distance in centimeters = Time / 58
      Distance in inches = Time / 148
Or you can utilize the speed of sound, since it is known that sound travels through air at about 344 m/s (1129 ft/s), you can take the time for the sound wave to return and multiply it by 344 meters (or 1129 feet) to find the total round-trip distance of the sound wave. Round-trip means that the sound wave traveled 2 times the distance to the object before it was detected by the sensor; it includes the ‘trip’ from the sonar sensor to the object AND the ‘trip’ from the object to the Ultrasonic sensor (after the sound wave bounced off the object). To find the distance to the object, simply divide the round-trip distance in half.

![400px-Ultrasonic_Sensor_Distance_Formula](https://user-images.githubusercontent.com/61703896/174466511-031ce89e-4b53-43fb-a9bc-dbfe26cdadd4.png)

## You Need to install 4 libraries 

Arduino.h
<br>
NewPing.h
<br>
SoftwareSerial.h
<br>
DFRobotDFPlayerMini.h

## You can check my [ppt](https://docs.google.com/presentation/d/1bNCLbX-0vshMBwTqYvA_Anl2mRlpFLoYSxc1NNlQqMg/edit?usp=sharing )





