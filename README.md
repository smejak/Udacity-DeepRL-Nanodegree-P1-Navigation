# Udacity-DeepRL-Nanodegree-P1-Navigation
This repository consists of my implementation of the first project from Udacity's Deep Reinforcement Learning Nanodegree course.
## Project details
This project consists of a reinforcement learning agent which solves the Banana navigation environment based on Unity machine learning problems. See [Unity ML-agents](https://github.com/Unity-Technologies/ml-agents) for more details.

The environment is considered solved when the agent receives a reward of +13 over 100 consecutive episodes. A reward of +1 is received whenever the agent collects a yellow banana and -1 whenever the agent collects a blue banana. 

There are four possible actions:

0. forward
1. backward
2. turn left
3. turn right

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. This information is used to determine the best actions.

## Getting started
The following section was taken from [Udacity's GitHub](https://github.com/udacity/deep-reinforcement-learning#dependencies) for its simple guide on how to get your local machine ready for reinforcement learning with Unity.
## Dependencies

To set up your python environment to run the code in this repository, follow the instructions below.

1. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__: 
	```bash
	conda create --name drlnd python=3.6
	source activate drlnd
	```
	- __Windows__: 
	```bash
	conda create --name drlnd python=3.6 
	activate drlnd
	```
	
2. Follow the instructions in [this repository](https://github.com/openai/gym) to perform a minimal install of OpenAI gym.  
	- Next, install the **classic control** environment group by following the instructions [here](https://github.com/openai/gym#classic-control).
	- Then, install the **box2d** environment group by following the instructions [here](https://github.com/openai/gym#box2d).
	
3. Clone the repository (if you haven't already!), and navigate to the `python/` folder.  Then, install several dependencies.
```bash
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

4. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment.  
```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

5. Before running code in a notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu.

## Instructions
To run this project on your local machine, clone this repository.
```bash
git clone https://github.com/smejak/Udacity-DeepRL-Nanodegree-P1-Navigation.git
```
Then, open the __Navigation.ipynb__ file and follow the instructions to train your own agent.
