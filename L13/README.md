# Lab 13: Reinforcement Learning with Q-Learning (Grid World Navigation)

This repository contains the Jupyter Notebook for Lab 13. The goal of this lab is to train an agent to successfully navigate a 4x4 Grid World environment manually using the Q-Learning algorithm.

## 📝 Overview

In this lab, we implemented a custom environment and a Q-learning agent from scratch to learn the optimal path from a start state to a goal state while avoiding obstacles. 

Key steps implemented include:
- **Environment Setup**: Creating a 4x4 `GridWorld` with specific start `(3,0)`, goal `(0,3)`, and obstacle `(0,0)`, `(1,1)` coordinates.
- **Environment Dynamics**: Implementing the `step()` function to update the agent's position based on actions (UP, RIGHT, DOWN, LEFT), handle boundary/obstacle collisions, and assign step penalties / goal rewards.
- **Q-Learning Agent Implementation**: 
  - Using an $\epsilon$-greedy policy (`epsilon = 0.2`) for action selection to balance exploration and exploitation.
  - Updating the Q-table progressively based on the Bellman equation update rule.
- **Model Training**: Training the agent for 100 episodes, tracking the total reward and the number of steps taken per episode.
- **Visualization & Evaluation**: Plotting learning curves (Total Reward per Episode & Number of Steps to Goal) to clearly observe the successful convergence of the Q-Learning algorithm to its optimal policy.

## 📂 Project Structure

- `6787074_Lab13_gridworld.ipynb`: The main notebook containing the GridWorld environment, Q-Learning agent, training loop, and evaluation visualizations.
- `L13_tic-tac-toe.ipynb`: An additional notebook related to earlier theoretical RL foundations.

## ⚙️ Requirements

To run this project, make sure you have the following Python libraries installed:
- `numpy`
- `matplotlib`
- `time`
