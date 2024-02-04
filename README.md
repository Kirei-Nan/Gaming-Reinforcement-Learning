
# Super Mario Bros PPO Agent

## Overview
This project uses Proximal Policy Optimization (PPO), a policy-based method, to train an intelligent agent to play the game Super Mario Bros. PPO is selected for its stability and efficiency in training compared to other policy gradient methods.

## Environment Setup
- Game: gym-super-mario-bros 7.3.2 on OpenAI Gym
- Simulator: Nes-py for virtual joypad integration
- RL Algorithm Library: Stable-Baselines3

## Custom Mario Environment
The Mario environment is wrapped to modify the reward function, including game score and a bonus for flag capture. The environment is reset upon death, with rendering and closing functions defined for game interactions.

## Preprocessing
The environment is vectorized using Stable-Baselines3 utilities to improve training speed and exploration. Frames are stacked to give the agent a sense of motion.

## Model Training
The PPO algorithm is configured with optimized hyperparameters. A custom callback function saves the best model during training.

## Results
The agent is trained in different difficulty levels of the game environment, showing robust performance and generalization. The study shows the importance of reward function design and the benefits of using multiple agents for training efficiency.

## Conclusions
Reinforcement Learning, particularly with PPO, proves to be environment-sensitive and resource-intensive. Future works include algorithm comparison and environment modeling studies.

## How to Use
Instructions on how to set up the environment, train the model, and test the trained agent are provided. Additionally, code snippets are given for clarity.

## Training Results and Videos
The `results` folder contains the training output and videos demonstrating the agent's performance in different environments.
