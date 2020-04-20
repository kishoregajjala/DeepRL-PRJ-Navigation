# DeepRL-PRJ-Navigation
This project repository contains my work for the Udacity's Deep Reinforcement Learning Nanodegree Project 1: Navigation.

### Project Description
For this project, we will train an agent to navigate (and collect bananas!) in a large, square world.The world contains both yellow and blue bananas.

### Reward
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. 

### State Space
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction

### Action
The agent has to learn how to best select actions. Four discrete actions are available, corresponding to:<br/>
. 0 - move forward.<br/>
. 1 - move backward.<br/>
. 2 - turn left.<br/>
. 3 - turn right.<br/>

### Project Goal
The goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas. 
The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

### Quick introduction about Deep Reinforcement Learning

To understand this implementation, you will have to have some understanding of Deep Reinforcement Learning. I recommend you  reading > Deep Reinforcement learning.

Reinforcement learning refers to goal-oriented algorithms, which learn how to attain a complex objective (goal) or maximize along a particular dimension over many steps; for example, maximize the points won in a game over many moves. They can start from a blank slate, and under the right conditions they achieve superhuman performance. Like a child incentivized by spankings and candy, these algorithms are penalized when they make the wrong decisions and rewarded when they make the right ones – this is reinforcement.

AlphaGo is a famous example of how Deep Reinforcement Learning achieve superhuman performance and defeated the world champion.

This navigation project implements a Value Based method called Deep Q-Networks

## The Environment
The details are taken from the Udacity's [Deep Reinforcement Learning Nanodegree program](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893/ "Deep Reinforcement Learning Nanodegree program").
The environment is based on Unity ML-agents. Please read more about ML-Agents by perusing the [GitHub repository](https://github.com/Unity-Technologies/ml-agents/ "GitHub repository title").

The project environment is similar to, but not identical to the Banana Collector environment on the [Unity ML-Agents GitHub page](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector/ "Unity ML-Agents GitHub page").

Follow the instructions below to explore the environment on your own machine! You will also learn how to use the Python API to control your agent.

###Step 1: Clone the DRLND Repository
If you haven't already, please follow the [instructions in the DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies/ "instructions in the DRLND GitHub repository") to set up your Python environment. These instructions can be found in README.md at the root of the repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.

(For Windows users) The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM such as Bootcamp or Parallels.

###Step 2: Download the Unity Environment
For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:

Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip/ "click here")
Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip/ "click here")
Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip/ "click here")
Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip/ "click here")
Then, place the file in the p1_navigation/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

(For Windows users) Check out this link if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to enable a virtual screen, and then download the environment for the Linux operating system above.)
