#Problem 1.5 of Chapter 1
Chenming Guo, 2011302430012, Physics

##Abstract
  Using Euler method with Python, solve the problem 1.5 of chapter 1.
<br/><br/>

##Introduction
###Problem 1.5
  Consider again a decay problem with two types of nuclei A and B, but now suppose that nuclei of type A decay into ones of type B, while nuclei of type B decay into type A. Strictly speaking, this is not a "decay" process, since it is possible for the type B nuclei to turn back into type A nuclei. A better analogy would be a resonance in which a system can tunnel or move back and forth between two states A and B which have equal energies. The corresponding rate equations are<br/>
![公式1](http://latex.codecogs.com/gif.latex?%5Cfrac%7BdN_A%7D%7Bdt%7D%20%3D%20%5Cfrac%7BN_B%7D%7B%5Ctau%7D%20-%20%5Cfrac%7BN_A%7D%7B%5Ctau%7D%2C) ![公式2](http://latex.codecogs.com/gif.latex?%5Cfrac%7BdN_B%7D%7Bdt%7D%20%3D%20%5Cfrac%7BN_A%7D%7B%5Ctau%7D%20-%20%5Cfrac%7BN_B%7D%7B%5Ctau%7D%2C)<br/>
where for simplicity we have assumed that the two types of decay are characterized by the same time constant, <img src="http://latex.codecogs.com/gif.latex?\tau." alt="" title="" /> Solve this system of equations for the numbers of nuclei, <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" /> and <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />, as functions of time. Consider different initial conditions, such as ![公式4](http://latex.codecogs.com/gif.latex?N_A%20%3D%20100%2C) ![公式5](http://latex.codecogs.com/gif.latex?N_B%20%3D%200%2C) etc., and take ![公式6](http://latex.codecogs.com/gif.latex?%5Ctau%20%3D%201) s. Show that your numerical results are consistent with the idea that the system reaches a stteady state in which <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" /> and <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" /> are constant. In such a steady state, the time derivatives <img src="http://latex.codecogs.com/gif.latex?dN_A/dt" alt="" title="" /> and <img src="http://latex.codecogs.com/gif.latex?dN_B/dt" alt="" title="" /> should vanish.<br/>

###The Euler Method
The principle of the Euler method is Taylor expansion. And the routine process is to substitute the given ordinary differential equation into the first-order derivative of the Taylor expansion and neglect infinitesimals of hiher order.
<br/><br/>

##Assignment
###Code 1
![Code 1](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%201.png)<br/>
[Code 1.py](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%201.py)<br/>
* Choose <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />0=100, <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />0=0, TA=TB=1. Result:
![Code 1 Result 1](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%201%20Result%201.png)<br/>
* Choose <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />0=100, <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />0=50, TA=TB=1. Result:
![Code 1 Result 2](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%201%20Result%202.png)<br/>
* Choose <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />0=100, <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />0=0, TA=1, TB=2. Result:
![Code 1 Result 3](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%201%20Result%203.png)<br/>

###Code 2
![Code 2](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%201.png)<br/>
[Code 2.py](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%202.py)<br/>
* Choose <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />0=100, <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />0=0, TA=TB=1, dt1=0.05, dt2=0.1. Result:
![Code 2 Result 1](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%202%20Result%201.png)<br/>
* Choose <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />01=100, <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />02=80, <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />=0, TA=TB=1, dt1=0.05, dt2=0.05. Result:
![Code 2 Result 2](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%202%20Result%202.png)<br/>
* Choose <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />01=100, <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" />02=80, <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />01=0, <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" />02=50, TA=TB=1, dt1=0.05, dt2=0.05. Result:
![Code 2 Result 3](https://github.com/gcmcpwork/compuational_physics_N2011302430012/blob/master/Exercise_04/Code%202%20Result%203.png)<br/>
<br/><br/>

##Conclusion
The Euler method can apply first-order differential equations and its results are in acceptable range.In this problem, <img src="http://latex.codecogs.com/gif.latex?N_A" alt="" title="" /> and <img src="http://latex.codecogs.com/gif.latex?N_B" alt="" title="" /> are constant finally when the system reachs equilibrium.In such a steady state,the time derivatives <img src="http://latex.codecogs.com/gif.latex?dN_A/dt" alt="" title="" /> and <img src="http://latex.codecogs.com/gif.latex?dN_B/dt" alt="" title="" /> should vanish.
<br/><br/>

##Thanks
Thanks to Professor Cai's guidance and help. And thanks to classmates for discussion.
