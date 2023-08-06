# Design of Optimal PID Controller for the Speed Control of DC Motor by Using Artificial Neural Network.
## ABSTRACT
The primary aim of this project is to control the speed of brushless DC motor using Artificial Neural Network (ANN) controller and PID controller. Detailed analysis is performed based on the simulation results of both the methods. A neural control-based speed control system of brushless DC motor is designed by analyzing the mathematical model of BLDC motor. Plant model identification is done in Simulink software of MATLAB to identify the ANN block of BLDC motor drive system. Reference control model is designed to give the ideal values of control parameters when the control system responds to the command signal. The performance results of PID controller and ANN controller are compared with reference model output of BLDC motor drive system in MATLAB Simulink environment. Comparative study concludes that ANN based speed control method eliminates the overshoot, reduces the settling time of the system response. It is observed that the ANN based simulation results are closer to the ideal reference control model response than PID based.

## MOTIVATION AND OBJECTIVE
Nowadays, the field of electrical power system control in general and motor control in particular has been researching broadly. The new technologies are applied to these in order to design the complicated technology system. One of these new technologies is Artificial Neural Network (ANNs) which based on the operating principle of human being nerve neural. It is composed of a large number of highly interconnected processing elements (neurons) working in unison to solve specific problems. ANNs, like people, learn by example. An ANN is configured for a specific application, such as pattern recognition or data classification, through a learning process. Learning in biological systems involves adjustments to the connections that exist between the neurons. This is true of ANNs as well. There are a number of articles that use ANNs applications to identify the mathematical DC motor model. Then, this model is applied to control the motor speed. The inverting forward ANN with two input parameters for adaptive control of DC motor ANNs are applied broadly because all the ANN signal are transmitted in one direction, the same as in automatically control system, the ability of ANNs to learn the sample, From the very beginning, it has been realized by systems theorists that most real-world dynamical systems are nonlinear. However, linearization's of such systems around the equilibrium states yield linear models, which are mathematically obedient. In particular, based on the superposition principle, the output of the system can be computed for any arbitrary input, and alternately, in control problems, the input, which optimizes the output in some sense, can also be determined with relative ease. In most of the adaptive control problems, where the plant parameters are assumed to be unknown, the fact that the latter occur linearly makes the estimation procedure straightforward. The fact that most nonlinear systems thus far could be approximated satisfactorily by linear models in their normal ranges of operation has made them attractive in practical contexts as well. It is this combined effect of ease of analysis and practical applicability that accounts for the great success of linear models and has made them the subject of intensive study for over four decades. In recent years, a rapidly advancing technology and a competitive market have required systems to operate in many cases in regions in the state space where linear approximations are no longer satisfactory. To cope with such nonlinear problems, research has been underway on their identification and control using artificial neural networks based entirely on measured inputs and outputs.
## OUTLINE OF THE PROJECT
1. The mathematical model of the PID controller and of the BLDC motor have been derived.
2. Using the model, a conventional controller has been designed in MATLAB for data collection.
3. A neural network controller has also been designed with MATLAB for supervised machine learning purposes.
4. The neural network has then been trained using 80% of the collected data from MATLAB by a back-propagation algorithm.
5. The trained neural network is then tested on the remaining data collected from MATLAB, based on which step-4 is repeated if necessary.
6. The traditional PID controller is replaced with the neural network controller and tested in real-time.
7. Finally, the performance of the proposed controller will be compared to the performance of the conventional BLDC motor controller for speed and accuracy.

## PURPOSE, SCOPE, AND APPLICABILITY
### PURPOSE
- To estimate the speed of the DC motor and control it, ANN can replace sensors speed in the control systems model. Using ANN, we don’t have to calculate the parameters of the motor when designing the control system. It may be revealed that an appreciable advantage of a control system using ANNs when parameters of the DC motor is variable during the operation of the motors. The satisfying ability of the system control with ANNs and ANN application can be used in adaptive controlling in the control system machine with the complicated load. To control the speed of DC Motor, experts used PID Controller fortuning the ANN to improve speed accuracy.
### SCOPE
- An ANN based adaptive controller performance is superior it still lacks with some limitations, which provides room for improvement. Such possible improvements are indicated below, as possible directions for further work. In the present work the number of hidden layers and the number of neurons in the hidden layer are chosen by trial and error, bearing in mind that the smaller the number, the better itis in terms of both memory and time taken to implement the ANN. Further research can be done to find the optimum number of hidden layers and number of neurons in the hidden layer. weights and biases updating feature of the ANN can compensate for both parameter changes and disturbances during operation. The uses of the adaptive learning rate in the proposed controller reduce the possibility of overshooting particularly during the transient conditions. The feedback provision in the modified ANN motor structure also enhances the stability of the system.
### APPLICABILITY
- Although the adaptive controllers' performance is superior, it still lacks some limitations, which provides room for improvement. As we know, the market potential increases with the increase in the efficiency of the system. Hence, further research can be done to improve the efficiency of the overall system during operation. Moreover, the efficient design of the controller may give a competitive advantage compared to the available systems.

## ACKNOWLEDGEMENT
I have taken efforts in this project. However, it would not have been possible without the kind support and help of many individuals and organization. I would like to extend my sincere thanks to all of them. I would like to express my sincere gratitude to my project guide “[Dr. Asim Halder]” for giving me the opportunity to work on this topic. It would never be possible for us to take this project to this level without his innovative ideas and his relentless support and encouragement. I would also like to give special thanks and appreciations to all my group mates for their kind co-operation support and encouragement which helped me a lot to complete my project within the limited time frame.
