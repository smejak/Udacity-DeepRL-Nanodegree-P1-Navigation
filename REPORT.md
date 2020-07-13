# Project 1 of the Udacity Deep Reinforcement Learning Nanodegree
## Learning Algorithm
### DQN
The learning algorithm used to train the agent is Deep Q-Learning, described in the paper [Human-level control through deep reinforcement learning](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf). Deep Q-Learning makes use of a feedforward neural network to substitute the Q-table, which is the primary component of basic Q-Learning. A DQN agent approximates the action-value function and acts as to maximise the expected reward over an episode. 
### Experience Replay
As described in the original [paper](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf), we make use of experience replay for two reasons:

* Greater data efficiency as one experience can be used to update the network weights multiple times
* Better learning resulting from randomly sampling the experiences instead of only learning from consecutive time steps

![Algorithm from the used from the [paper](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf)](/algo.png)
## Implementation
The implementation of the DQN can be found in the files model.py and dqn_agent.py.

model.py makes use of PyTorch to create a feedforward neural network with 2 fully connected layers of 128 units each. The input to the network is the state (37 nodes corresponding to state dimensions) and the output of the network corresponds to the 4 available actions.
NOTE: All of the parameters can be adjusted for any environment.

dqn_agent.py consists of a class constructor for the deep q-learning agent as well as for the replay memory.

### Hyperparameters
Hyperparameters for the DQN agent can be found in dqn_agent.py.

Parameters used for the training algorithm:
* maximum number of timesteps per episode = 1000
* epsilon_start = 1.0
* epsilon_end = 0.01
* epsilon_decay = 0.95

## Results
```
Episode 100	Average Score: 3.12
Episode 200	Average Score: 8.46
Episode 300	Average Score: 12.04
Episode 358	Average Score: 13.01
Environment solved in 258 episodes!	Average Score: 13.01
```
![](/learning_curve.png)
The results show that the environment has been successfully solved as the average score over 100 consecutive episodes was more than +13.

### Additional results
I was curious to see how the agent would improve if the training did not terminate after first solving the environment. After training it for 600 episodes,  
