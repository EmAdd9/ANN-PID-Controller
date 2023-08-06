# PLANT MODEL OF BLDC MOTOR
Digital computer simulation model of BLDC motor drive has been developed by
using Simulink MATLAB software as shown in Fig 6. Run this simulation. After
this in MATLAB workspace the inputs u1 and y1 are declared to x variable and y
is set as output variable assigned for t variable. The ANN is trained by
‘nnnstart’ command in fool fitting app in the MATLAB software. Numbers of
hidden layers are chosen as 10 and training is done. After training the ANN
block is placed in the Simulink diagram of speed control of BLDC motor as shown.
![BLDC-Motor-Plant-Model](<https://github.com/EmAdd9/ANN-PID-Controller/blob/dd425a567245143376868047d0164dbbacd12380/Design%20and%20Implementation/BLDC-Plant-Model.png>)

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
From equation (19),  𝑒−𝑡𝑠𝑇𝑚 = 1 - 𝑌𝑚(𝑡) (20)
0.02 ≥ 1 - 𝑌𝑚(𝑡) (21)
ln(0.02) = −𝑡𝑠𝑇𝑚 𝑇𝑚=−𝑡𝑠ln (0.02)=−0.001ln (0.02)=2.5562×10−4𝑠𝑒𝑐 (22) 
Since 𝐺(𝑠)𝑠=0=910 from (16) then the reference model is
𝐺𝑚(𝑠)= 910(2.5562×10−4)𝑠+1 (23) 
𝐺𝑚(𝑠)=(910)3.9121×103𝑠+3.9121×103 (24) 
Using pole zero mapping discretization method, 𝐺𝑚(𝑧)=𝑌𝑚𝑅(𝑧)=294.6580𝑧−0.6762 (25) Eq. (25) is transfer function for reference control model.

# NEURAL NETWORK TRAINING
Training a Neural Network means finding the appropriate Weights of the Neural Connections thanks to a feedback loop called Gradient Backward propagation. Figure 7 shows the neural network training. In the system identification stage a neural network plant model must be developed before the controller is used. The plant model predicts future plant outputs. The specifications of the plant model are given in figure.
![Neural-Network-Training](<https://github.com/EmAdd9/ANN-PID-Controller/blob/dbf33cbf23acca30d5b2a478be2a49ac497e462b/Design%20and%20Implementation/Training-Summary.png>)

## Training Result
![Neural-Network-Training-Result](<https://github.com/EmAdd9/ANN-PID-Controller/blob/dbf33cbf23acca30d5b2a478be2a49ac497e462b/Design%20and%20Implementation/Training-report.png>)

## Regression Plot
![Regresiion Plot](<https://github.com/EmAdd9/ANN-PID-Controller/blob/dbf33cbf23acca30d5b2a478be2a49ac497e462b/Design%20and%20Implementation/Regression-Plot.png>)

## Performance Plot
![Regresiion Plot](<https://github.com/EmAdd9/ANN-PID-Controller/blob/dbf33cbf23acca30d5b2a478be2a49ac497e462b/Design%20and%20Implementation/performace-plot.png>)

## Error Histogram
![Error-Histogram](<https://github.com/EmAdd9/ANN-PID-Controller/blob/dbf33cbf23acca30d5b2a478be2a49ac497e462b/Design%20and%20Implementation/erroe-histogram.png>)

## Function Fitting Neural Network
![Function-Fitting-NN](<https://github.com/EmAdd9/ANN-PID-Controller/blob/dbf33cbf23acca30d5b2a478be2a49ac497e462b/Design%20and%20Implementation/Function-Fitting-NN.png>)

## Simulink Model of ANN Controller and BLDC Motor
![Function-Fitting-NN](<https://github.com/EmAdd9/ANN-PID-Controller/blob/1ec4829b0d6c532e37f14d46ecaf6f26add480b6/Design%20and%20Implementation/Simulink%20Model%20for%20ANN%20Controlled%20BLDC%20motor.png>)

## Process:
Digital computer simulation model of BLDC motor drive has been developed by using Simulink MATLAB software as shown in Fig 6.Run this simulation. After this in MATLAB workspace the inputs u1 and y1 are declared to x variable and y is set as output variable assigned for t variable. The ANN is trained by ‘nnstart’ command in nftool fitting app in the MATLAB software. Numbers of hidden layers are chosen as 10 and training is done. After training the ANN block is placed in the Simulink diagram of speed control of BLDC motor as shown.Problems encountered and solutions

### Problem encountered: - 
i) Control of DC motor speed
ii) Interface of DC motor with software (MATLAB/SIMULINK)
iii) To acquire data from the DC motor

### Solutions: -
i) Use of ANN controller to the system
ii) Implementation of DAQ card to the control board
iii) Use of encoder from the DC motor to the control board
