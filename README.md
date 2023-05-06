# SelfBalancingRobot
Inverted Wheeled Pendulum is a non-linear system. This specific type of robot consists of a body above two wheels with no balancing support. Its main task is to maintain the pitch angle in a vertical position to stabilize the structure.

## Mechanical Design

![image](https://user-images.githubusercontent.com/76494996/236623901-3da85d5c-4583-4d80-a1b7-4c641038be7b.png)

## Electrical Design

![image](https://user-images.githubusercontent.com/76494996/236624001-a28dfd74-f443-4a09-874f-73b266476c49.png)

## Block diagram
In this section, let's illustrate the control of the system using a block diagram. The PID controller takes the disorientation error as input and outputs motor commands in the form of voltage. 
![image](https://user-images.githubusercontent.com/76494996/236623743-f255892b-7b23-4f52-a72e-f2d0089e9203.png)

## Command
At each sampling time, we apply the following command.

command= Kp *Error+ Ki *SumErrors+ Kd *(error- PreviousEror)/0.001

## Software
### organigram 
![image](https://user-images.githubusercontent.com/76494996/236624154-d7db1fd9-a0a3-442a-9146-317fbf71e082.png)
