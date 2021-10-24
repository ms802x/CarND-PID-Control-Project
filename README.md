# PID Control Project
In this project, I will be using  C++ to program PID controller, that controlls the steering of a veichle in a racing track.  

### What is PID?
PID stands for Proportional-Integral-Derivative, and it is used for correcing error and increasing the stabiity of a system. The PID controller is made of three components P, I and D. Each of which serve in decreasing the stearing angle error. In this project we were given the Cross Track Error(CTE), which represent the distance of the vehicle from the trajectory. 

<p align="center">
  <img width="460" height="300" src="https://www.gstatic.com/education/formulas2/397133473/en/pid_controller.svg">
</p>

- The  proportional component P,  minmize the error linearly with a constant factor Kp(It may overshot)
- The Integral factor I, summs all the error observed by the system which helps in reducing the bias (sush as wrong car wheels aligment.
- The differential component,it helps in minmizing overshot. taking two measurment of CTE in 1 second of time

### Parmater Tuning 

I have set my paramters manually till I got a good result. My result are not the best and parameters need more tuning, however, the car will not leave the lane with these paramters.

- kp=-0.4
- kd=-3.4
- ki=-0.004
