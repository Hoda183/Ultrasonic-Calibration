# Task 1 Measurements
##  Circuit design

[Tinkercad circuit](https://www.tinkercad.com/login?next=%2Fthings%2F4TwnLUDbhPA-task-1-measure)

The ultrasonic sensor includes 4pins: 

* VCC: needs to be connected to VCC (5V). 

* GND: needs to be connected to GND (0V). 

* TRIG: this pin receives the control signal (pulse) from Arduino.  

* ECHO: this pin sends a signal to Arduino. Arduino measures the duration of pulse to calculate distance.  

![Circuit Design](https://github.com/user-attachments/assets/507352eb-700b-47e1-b45e-deefb87535ad)

 
# How It Works: 

1. Micro-controller generates a 10-microsecond pulse on the TRIG pin 

2. The ultrasonic sensor automatically emits the ultrasonic waves 

3. The ultrasonic wave is reflected after hitting an obstacle 

4. The ultrasonic sensor :
   * Detects the reflected ultrasonic wave 
   * Measures the travel time of the ultrasonic wave 

5. Ultrasonic sensor generates a pulse to the ECHO pin The duration of the pulse is equal to the travel time of the ultrasonic wave 

6. Micro-controller measures the pulse duration in the ECHO pin, and then calculate the distance between sensor and obstacle. 
