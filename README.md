# Udacity Deep RL nanodegree - Project 1: Navigation
This is the first project of the Udacity deep reinforcement learing Non-degree program. The main goal of this project is to train an agent that navigate in a squared world to collect yellow bananas and avoid the blue ones. The agent recieves a reward +1 for every collected yellow banana and a reward -1 if the collected banana is blue. Thus, the goal is to train the agent such that it collects as many yellow bananas as possible while avoiding blue bananas.

## State and Action Spaces

The state space is a vector of 37 continuous values containing the agent's speed, along with ray-based perception of objects around the agent's forward direction. Given the information in the state space, the agent has to learn how to pick the best action in every situation. The action space is discrete and has the following allowed movements:
* forrward.
* backward.
* left.
* right.

The task is episodic and considered solved if the agent achieves an average score of +13 over 100 consecutive episodes.

### Repository structure
The code is structured as follows: 
* **Navigation.ipynb**: this is where the deep rl agent is trained.
* **agent.py**: this module implements a class to represent a vanilla dqn agent.
* **model.py**: this module contains the implementation of the neural network approximating the action value function.
* **checkpoint.pth**: this is the binary containing the trained neural network weights.

### Dependencies
* python 3.6
* numpy: install with 'pip install numpy'.
* PyTorch: install by following the instructions [here](https://github.com/reinforcement-learning-kr/pg_travel/wiki/Installing-Unity-ml-agents-on-Windows).
* ml-agents: install by following instructions [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation-Windows.md).

## Getting Started
In cell 2 of Navigation.ipynb we import the Unity environment from a remote server. For a local installation of the Unity ml-agents, please refer to the following two sources:
* [Linux, Mac](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md)
* [Windows 10](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation-Windows.md)

## Instructions
This is a jupyter notebook project. To run the code and train the deep reinforcement learning agent, you simply execute each of the cells in **Navigation.ipynb**. After training, the average score per hundred episodes will be displayed.

