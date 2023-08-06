# PLANT MODEL OF BLDC MOTOR
Digital computer simulation model of BLDC motor drive has been developed by
using Simulink MATLAB software as shown in Fig 6. Run this simulation. After
this in MATLAB workspace the inputs u1 and y1 are declared to x variable and y
is set as output variable assigned for t variable. The ANN is trained by
‘nnnstart’ command in fool fitting app in the MATLAB software. Numbers of
hidden layers are chosen as 10 and training is done. After training the ANN
block is placed in the Simulink diagram of speed control of BLDC motor as shown.
![BLDC-Motor-Plant-Model](<link>)

## REFERENCE CONTROL MODEL OF BLDC MOTOR
Reference control model will give ideal system response which will be compared
with the response of ANN controller and PID controller.
Response of neural control BLDC motor is compared with ideal response of
reference control model. Reference control model is designed by considering the
following performance criteria.
(1) No overshoot
(2) Zero steady state error
(3) Take 0.001 sec. as a settling time
Considering reference model as a first order model, the transfer function is
given by [11],
𝑌(𝑆)𝑅(𝑆)=1𝑇𝑚𝑆+1 (18)
Consider Unit Step as a reference input. Taking Inverse Laplace Transform,
For t ≥ 0,
𝑌𝑚(𝑡)=1−𝑒−𝑡𝑠𝑇𝑚 (19)
For zero steady state error and 𝑒−𝑡𝑠𝑇𝑚 = ±2% criteria, the final response value is the same as the reference input.
From equation (19),
𝑒−𝑡𝑠𝑇𝑚 = 1 - 𝑌𝑚(𝑡) (20)
0.02 ≥ 1 - 𝑌𝑚(𝑡) (21)
ln(0.02) = −𝑡𝑠𝑇𝑚 𝑇𝑚=−𝑡𝑠ln (0.02)=−0.001ln (0.02)=2.5562×10−4𝑠𝑒𝑐 (22) Since 𝐺(𝑠)𝑠=0=910 from (16) then the reference model is
𝐺𝑚(𝑠)= 910(2.5562×10−4)𝑠+1 (23) 𝐺𝑚(𝑠)=(910)3.9121×103𝑠+3.9121×103 (24) Using pole zero mapping discretization method, 𝐺𝑚(𝑧)=𝑌𝑚𝑅(𝑧)=294.6580𝑧−0.6762 (25) Eq. (25) is transfer function for reference control model.

# NEURAL NETWORK TRAINING
Training a Neural Network means finding the appropriate Weights of the Neural Connections thanks to a feedback loop called Gradient Backward propagation. Figure 7 shows the neural network training. In the system identification stage a neural network plant model must be developed before the controller is used. The plant model predicts future plant outputs. The specifications of the plant model are given in figure.
![Neural-Network-Training](<link>)