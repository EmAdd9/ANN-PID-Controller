# -------------------------Result-------------------------- 
## Performance Comparison between PID, ANN and Reference Model
![rport](https://github.com/EmAdd9/ANN-PID-Controller/blob/31d29d8e26a0f6734554af855b746586e8208b8b/Result-Analysis/pid-ann-ref_model.png)

## Output of reference model
![output](https://github.com/EmAdd9/ANN-PID-Controller/blob/31d29d8e26a0f6734554af855b746586e8208b8b/Result-Analysis/Settling-Time-0.3ms.png)
### Output of reference model. Settling time= 0.3 msec
The speed response of reference model is shown in fig The simulation result shows that the settling time of the reference system is about 0.3 msec along with zero overshoot in the response. To perform the simulation the step time and set time is taken as 0.00001 sec and 13650 respectively.

## Output of PID controller
![output](https://github.com/EmAdd9/ANN-PID-Controller/blob/31d29d8e26a0f6734554af855b746586e8208b8b/Result-Analysis/Settling-timw-1.7ms.png)
### Output of PID Controller. Settling time= 1.7 sec
The response of PID controller for the BLDC system is depicted in this fig. In this case the settling of the system is measured as around 1.7 sec which can be seen from the graph. Moreover, the response of the PID controller shows the overshoot of the response around 0.219 %. It can be clearly seen that the settling time and the overshoot of the BLDC motor controlled by PID controller is much higher than that of the reference model.

## Output of ANN controller
![output](https://github.com/EmAdd9/ANN-PID-Controller/blob/31d29d8e26a0f6734554af855b746586e8208b8b/Result-Analysis/Settling-time-0.9ms.png)
### Output of ANN Controller. Settling time= 0.9 msec
The output response of the BLDC motor with ANN controller is shown in fig. In this case also the set point of the speed is taken as 13650. The simulation result shows that the settling time of the response here in this case is around 0.9 msec which is better than the case of PID controller but it is more than the case of reference model. Furthermore, the response shows no overshoot in ANN based system unlike the PID based system. Therefore, it may be said that the ANN controller is more effective that the PID controller for the speed control of BLDC motor.
