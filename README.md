# MDP REPRESENTATION

## AIM:
### To represent a Markov Decision Process(MDP) problem in the following ways.
### 1) Text representation
### 2) Graphical representation
### 3) Python - Dictonary representation
## PROBLEM STATEMENT:
### To develop an environment in which a person is finding the class The goal is to reach the correct class.
## Problem Description
### The agent has to reach the goal class by taking the correct step towards the goal without drifting away from the path. After reaching the goal the agent will be rewarded if not then no reward will be provided.
## State Space:
### {0,1,2,3}
## Sample State:
### 0 -> class1
### 1 -> class2
### 2 -> class3
### 3 -> class4
## Action Space:
### {1,2}
## Sample Action:
### 1 -> Moving right
### 2 -> Moving left
## Reward Function:
###  Agent reached class3 state: reward=+1
###   other class reward=0
### Graphical Representation:
![po1](https://github.com/user-attachments/assets/2d7594a1-08b3-405a-a51e-ca8414cef0e3)


## PYTHON REPRESENTATION:
```
class = { 
    class 1
  0:{
     1:[(0.7 , 1 , 0,False),
       (0.3 , 0 , 0 , False)],
     2:[(0.7 , 0 , 0,False),
       (0.3 , 1 , 0 , False)] 
  },
    class 2
  1:{
     1:[(0.7 , 2 , 0,False),
       (0.3 , 0 , 0 , False)],
     2:[(0.7 , 0 , 0,False),
       (0.3 , 2 , 0 , False)]
  },
    class 3
  2:{
      1:[(0.7 , 3 , 1,True),
        (0.3 , 1 , 0 , False)],
      2:[(0.7 , 1 , 0,False),
        (0.3 , 3 , 1 , True)]
  },
    Rclass 4
  3:{
      1:[(0.7, 3 , 0, True),
        (0.3 , 2 , 0 , False)],
      2:[(0.7, 2 , 0, False),
        (0.3 , 3 , 0 , True)]
  }
}
class
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/f35aa83a-4346-4e81-a6a8-cd6e48149b72)


## RESULT:
### Hence we have created an environment suitable for the above mentioned problem.
