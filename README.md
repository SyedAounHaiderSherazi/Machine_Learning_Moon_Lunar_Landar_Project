# Machine_Learning_Moon_Lunar_Landar_Project

# 🚀 Lunar Lander - Reinforcement Learning Project

This project is based on the **Lunar Lander** problem from the final lab of the **DeepLearning.AI Reinforcement Learning Specialization** on Coursera. It utilizes **Deep Q-Learning** to train an agent to land a lunar module safely between two flags on a simulated moon surface.

---

## 📌 Problem Statement

The objective is to **control a lunar lander module** and help it land softly on the designated landing pad using discrete action space. The lander must avoid crashing or flying off-screen while minimizing fuel consumption and maximizing stability.

---

## 🎮 Environment

- **Environment Used**: `LunarLander-v2` from [OpenAI Gym](https://www.gymlibrary.dev/environments/box2d/lunar_lander/)
- **Observation Space**: 8-dimensional state vector (position, velocity, angle, etc.)
- **Action Space**:  
  - `0`: Do nothing  
  - `1`: Fire left engine  
  - `2`: Fire main engine  
  - `3`: Fire right engine

---

## 🧠 Algorithm Used

### Deep Q-Learning (DQN)
- Approximates Q-values using a neural network
- Uses **Experience Replay Buffer** to learn from past experiences
- Implements a **Target Network** for stable learning
- Employs **epsilon-greedy policy** for exploration vs exploitation

---

## 🏁 Performance

- The trained agent was able to **successfully land** the lunar module consistently after training.
- Rewards exceeded the **solving threshold of 200+ average score** over 100 episodes.
- Demonstrates key RL concepts such as exploration, reward maximization, and learning stability.

---

## 🧪 Dependencies

```bash
pip install gym[box2d] numpy matplotlib torch
