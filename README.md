[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

[image2]: Score_plot.png "Score Plot"

# Project 1: Navigation

### Introduction

This project is part of the Udacity [Deep Reinforcement Learning Nanodegree Program](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893). It has the environment for Mac OSX. 

The goal is to create and train an Agent to navigate and collect bananas in a large, square world.  

![Trained Agent][image1]

### Environment Details

The envoronment is built using [Unity Machine Learning Agents](https://github.com/Unity-Technologies/ml-agents) (**ML-Agents**), which is an open-source Unity plugin that enables games and simulations to serve as environments for training intelligent agents. 
The project environment, provided by Udacity is similar to, but not identical to the Banana Collector environment on the [Unity ML-Agents GitHub page](https://github.com/Unity-Technologies/ml-agents). The environment has been downloaded from [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip) for Mac OSX.

In this environment, an Agent navigates a large, square world collecting bananas. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

#### State and Action spaces

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

### Getting Started

1. Follow the instructions [here](https://github.com/udacity/Value-based-methods#dependencies) to setup the python environment. It has instructions to install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.
2. Download this repository (only for Mac OSX), it has the environment included. So for Mac OSX, step 3 can be skipped.
3. Download the environment from one of the links below (For Mac OSX, this step can be skipped as the environment is already included in this repo).  Select the environment corresponding to the required operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

4. Place the file in the repository (downloaded in step 2) and unzip (or decompress) the file. 

### Instructions

The environment just set up has the files and tools to allow the training of the agent.

Start the Jupyter Notebook server by running the commands below (in Mac OSX). A new browser tab will open with a list of the files in the current folder.

```
$ source activate drlnd
$ jupyter notebook
```

Follow the instructions in `Navigation.ipynb` to get started with training your own agent!  

The task of collecting 13 bananas,on average,(sampled from 100 episodes) was completed using Deep Q-Learning Network with modifications.

```
Environment solved in 406 episodes!	Average Score: 13.00
```
![Score Plot][image2]

For more details see the [Report](https://github.com/tamoghna21/DeepRL-Project-Navigation/blob/main/Report.pdf).
