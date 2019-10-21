# Udacity Deep Reinforcement Learning - Project 2 - Continuous Control
----------------------------------------------------------------------

This is the report for Project 2 - Continuous control from the Deep Reinforcement Learning Nanodegree of Udacity. 

## Project details

The task is to train an agent to maintain the position of a double-jointed arm at a moving target location for as many time steps as possible. The task is continuous, although the episodes end after a certain time.

A reward of 0.1 is provided for each step that the agent’s hand is in the goal location. In order to solve the environment, the agent must pick an average score of 30+ over 100 consecutive episodes. The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector must be a number between -1 and 1.

## Getting Started

The top level of the project has been developed as a Jupyter notebook (`Navigation.ipynb`) in Python 3, thus make sure that you have a running Python and Jupyter working installation.

The world is provided as an Unity environment and is external to the project itself. To install the environment you will need a distribution of the ml-agents package from Unity. Please follow the installation instructions there, as this may change, in our case we followed the installation instructions of Udacity.

The agent is provided in `dpqg_agent.py`, and the underlying neural network models in `model.py` (both these files were obtained from Udacity Qnetwork project and tweaked). For these to run one needs to install Pytorch; other packages that need to be imported directly are numpy, and matplotlib. To install them, please run

`pip install numpy matplotlib pytorch`

In addition all these packkages will have dependencies themselves, which need to be satisfied before proceeding. A complete list of all the dependencies can be found in `requiriments.txt`, and istalled using

`pip requirements.txt`

## Instructions

The notebook is pretty much self-contained. It contains only three cells. 

- Run the first one one to set up the angent and the environment itself.
- The second one is optional, provides some information about the environment and basic usage interface of the agent and its interactions with the environment, as well as an example of how to use the agent. This can be used to evaluate the trained or untrained agents. A window should pop up that allows you to observe the agent, as it acts in the environment.
- The third one provides the code for the training itself, run this if you want to train the agent.
