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

### The Environment
#-
The environment is based on Unity ML-agents. Please read more about ML-Agents by perusing the [GitHub repository](https://github.com/Unity-Technologies/ml-agents/ "GitHub repository title").

The project environment is similar to, but not identical to the Banana Collector environment on the Unity ML-Agents GitHub page.

