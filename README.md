# DQN-DDQN

## Overview

This project implements Deep Q-Networks (DQN) and Double DQN agents to play the Atari Breakout game using the OpenAI Gym environment. The primary goal is to understand and apply deep reinforcement learning techniques with pixel-level environment information and to experiment with recurrent state encoding for improved performance.

---

## Features

- **DQN Implementation:** Standard Deep Q-Network agent.
- **Double DQN:** Enhanced agent with reduced overestimation bias.
- **Recurrent State (Extra Credit):** Optional DQNLSTM agent utilizing LSTM to encode history.
- **Training Environment:** Atari Breakout via OpenAI Gym.
- **Performance Targets:**  
  - DQN: Mean score of 8  
  - Double DQN: Mean score of 10  
  (within 2000–2500 episodes)

---

## Getting Started

### Prerequisites

- Python 3.7
- PyTorch 1.10.2
- OpenAI Gym
- Jupyter Notebook
- (Recommended) GPU-enabled environment (Google Colab or Google Cloud)

> **Note:** Running 2000+ episodes is computationally expensive and may take 4+ hours.

---

## Code Structure

- `MP5.ipynb` — Main notebook for implementing and training DQN and Double DQN.
- `agent.py` — DQN agent code.
- `agent_double.py` — Double DQN agent code.
- `config.py` — Hyperparameter configuration.
- `MP5_DQNLSTM_EC.ipynb`, `agent_lstm.py` — (Extra Credit) DQN with LSTM support.

---

## Assignment Goals

- Understand how Deep RL agents learn directly from raw pixel data.
- Implement and train DQN and Double DQN agents.
- Experiment with hyperparameters in `config.py` (optional).
- (Extra Credit) Implement and analyze a DQNLSTM agent or extend to other Atari games.

---

## Performance Milestones

| Agent         | Target Mean Score | Episodes         |
|---------------|------------------|------------------|
| DQN           | 8                | ~2000            |
| Double DQN    | 10               | ~2200            |
| DQNLSTM (EC)  | 8                |                  |

**Sample reward progression:**  
(DQN) 2000 episodes → mean score ≈ 8.6  
(Double DQN) 2200 episodes → mean score ≈ 10.1

---

## Useful References

- [Official DQN PyTorch Tutorial](https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html)
- [DQN Paper (Nature, 2015)](https://www.nature.com/articles/nature14236)
- [Double DQN Paper](https://arxiv.org/abs/1509.06461)
- [Medium DQN Tutorial](https://medium.com/@philtabor/deep-q-learning-tutorial-step-by-step-dqn-with-pytorch-54d3d159c054)

---

