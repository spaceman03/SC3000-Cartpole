# Cartpole Project
This repository contains the implementation of a classic reinforcement learning problem, Cartpole, using Q-learning and Deep Q-Networks (DQN). The Cartpole environment is a common benchmark problem where the objective is to balance a pole on a cart by applying forces to the cart.

## Introduction
In this project, we explore the Cartpole problem using two different Q-learning implementations with varying learning rates and a Deep Q-Network (DQN) approach. The goal is to compare the performance of these algorithms in terms of their ability to balance the pole over time.

## Environment
The CartPole environment is a part of the [OpenAI Gym library](https://www.gymlibrary.dev/environments/classic_control/cart_pole/), which provides a standard interface for a wide variety of reinforcement learning tasks. The state space consists of four variables: cart position, cart velocity, pole angle, and pole velocity at tip. The agent's actions are to move the cart left or right. The environment provides a reward of +1 for every time step the pole remains upright.

## Algorithms
### Q-learning
Q-learning is a model-free reinforcement learning algorithm that seeks to learn a policy, which tells an agent what action to take under what circumstances. We implemented Q-learning with two different learning rates:
- Q-learning (Low Learning Rate: 0.01)
- Q-learning (High Learning Rate: 0.65)
The learning rate determines how quickly the agent updates its knowledge about the environment.

### Deep Q-Network (DQN)
DQN is a more advanced method that uses a neural network to approximate the Q-value function. It is particularly useful in environments with large state spaces. Our implementation includes experience replay and a target network to stabilize training.

## Results
Both Q Learning (Learning rate: 0.65) and DQN are able to acheive a total reward of 500 for 100 episodes, while Q Learning (Learning rate: 0.01) was able to acheive a total reward of 495 for 100 episodes.

