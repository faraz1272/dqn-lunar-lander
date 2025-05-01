# DQN Lunar Lander

A Deep Q-Learning (DQN) agent trained to solve the LunarLander-v3 environment using PyTorch and OpenAI Gym. This project demonstrates reinforcement learning concepts such as experience replay, target networks, and epsilon-greedy exploration strategy.

---

## 🚀 Environment

- **Environment**: `LunarLander-v3` from OpenAI Gym
- **State Space**: 8 continuous variables
- **Action Space**: 4 discrete actions (do nothing, fire left engine, fire main engine, fire right engine)

---

## 🧠 Model Architecture

A simple fully connected feedforward neural network:

- `Input Layer`: 8 units (state size)
- `Hidden Layers`: 2 layers with 64 units each and ReLU activations
- `Output Layer`: 4 units (action values)

---

## 🛠️ Features

- Deep Q-Learning with target network updates
- Experience replay buffer
- Epsilon-greedy exploration with decay
- Training and loss monitoring
- Model checkpointing (`.pth` file)

---

## 📈 Training

The agent was trained for `1000` episodes with the following settings:

- Learning Rate: `0.001`
- Discount Factor (γ): `0.99`
- Replay Buffer Size: `10,000`
- Batch Size: `64`
- Epsilon Decay: `0.995` with `ε_min = 0.01`

### Plots for Training Rewards and Training Loss:
![image](https://github.com/user-attachments/assets/d485039f-47c3-44d1-bf56-b3d29d93a8ba)

---


## 💻 Getting Started

### 1. Install dependencies
```bash
pip install -r requirements.txt

