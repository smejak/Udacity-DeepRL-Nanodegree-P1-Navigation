# Project 1 of the Udacity Deep Reinforcement Learning Nanodegree
## Learning Algorithm
### DQN
The learning algorithm used to train the agent is Deep Q-Learning, described in the paper [Human-level control through deep reinforcement learning](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf). Deep Q-Learning makes use of a feedforward neural network to substitute the Q-table, which is the primary component of basic Q-Learning. A DQN agent approximates the action-value function and acts as to maximise the expected reward over an episode. 
### Experience Replay
As described in the original [paper](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf), we make use of experience replay for two reasons:

* Greater data efficiency as one experience can be used to update the network weights multiple times
* Better learning resulting from randomly sampling the experiences instead of only learning from consecutive time steps
