# DQN - Navigation-project

This project is an implementation of [DQN paper](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf)



![](banana_col.gif)

## Environment details
You will train an agent to collect bananas in a large, square world.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- ```0``` - move forward.
- ```1``` - move backward.
- ```2``` - turn left.
- ```3``` - turn right. 

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

## Installation

1. Download the environment from one of the links below. You need to select only the environment for your operating system:

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
(For Windows users) Check out this [link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a [virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use this [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the DRLND GitHub repository, in the ```p1_navigation/``` folder, and unzip (or decompress) the file.

3. Make sure you install Anaconda. You can download it from [here](https://www.anaconda.com/distribution/)

4. Now you can create your environment. Lets call our environment ```DRLND```
  
   Linux,Mac
   ```
   conda create --name drlnd python=3.6
   source activate drlnd
   ```
   Windows
   ```
   conda create --name drlnd python=3.6 
   activate drlnd
   ```
 5. We will be working with pytorch version 0.4.0 (an early version), so make sure that you install this version of pytorch:
   ```
   conda install pytorch=0.4.0 -c pytorch
   ```
 6. Perform a minimal installation of the [OpenAI Gym environment](https://github.com/openai/gym)
 
 7. Use command ```pip install``` and use it with all dependencies of the requirements.txt file
 
 8. Create a Python execution backend for Jupyter for the drlnd environment 
   ```
   python -m ipykernel install --user --name drlnd --display-name "drlnd"
   ```
 AND you are ready to use the environments

## Instructions
Follow the instructions in ```Navigation.ipynb``` to get started with training your own agent!

## Run the code
Execute the cells inside Navigation.ipynb file in sequential order so to proceed with training the agent. Tweak the hyperparameters to get different results. No need of GPU as this project is fast enough with CPU power.

