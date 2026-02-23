# ML Research: Intelligent Network Protocol Prioritization

This project focuses on applying Machine Learning and Reinforcement Learning techniques to analyze and prioritize network protocol traffic using Wireshark data.

The goal is to build an intelligent system that learns protocol behavior patterns and dynamically assigns priority levels based on frequency and importance.

---

## 📂 Dataset

Wireshark network traffic dataset used for training and experimentation:

🔗 Dataset Link:  
https://www.kaggle.com/datasets/rajtharani/wireshark1

The dataset contains:
- Timestamped protocol usage data
- Protocol counts
- Network traffic patterns
- Structured CSV logs exported from Wireshark

---
## 🚀 Project Overview

This research explores two main approaches:

### 1️⃣ Time Series Modeling (GRU)

We use a GRU (Gated Recurrent Unit) network to:
- Model sequential protocol traffic patterns
- Predict future protocol counts
- Capture temporal dependencies in network traffic

Why GRU?
- Efficient for sequential data
- Lower computational cost compared to LSTM
- Suitable for real-time inference scenarios

---
### 2️⃣ Reinforcement Learning (PPO)

We implement Proximal Policy Optimization (PPO) to:

- Dynamically assign protocol priorities
- Optimize Quality of Service (QoS)
- Learn from reward signals based on protocol importance

Reward function considers:
- Frequency
- Protocol criticality
- Traffic distribution

The environment simulates protocol state transitions and learns optimal prioritization policies.

---
## 🧠 Core Concepts Used

- Time Series Forecasting
- Sequence Modeling
- Reinforcement Learning
- PPO (Policy Gradient Method)
- Reward Shaping
- Network Traffic Analysis
- Feature Engineering
- Data Normalization

---
## 🛠 Tech Stack

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Stable-Baselines3 (PPO)
- Scikit-learn

---
## ⚙️ Project Structure
ml-research/
│
├── data/ # Dataset files (Wireshark CSV)
├── preprocessing/ # Data cleaning and normalization scripts
├── gru_model/ # GRU time-series implementation
├── rl_environment/ # Custom RL environment
├── ppo_training/ # PPO agent training
├── evaluation/ # Metrics and performance analysis
└── main.py # Entry point

--
## 📊 Model Pipeline

1. Data Collection (Wireshark logs)
2. Data Cleaning & Aggregation
3. Feature Scaling & Sequence Creation
4. GRU Model Training
5. Custom RL Environment Setup
6. PPO Training
7. Performance Evaluation

---
## 📈 Evaluation Metrics

For GRU:
- MSE (Mean Squared Error)
- MAE
- Trend stability

For PPO:
- Cumulative reward
- Policy convergence
- Priority assignment accuracy

---
## 🔬 Research Focus

This project aims to explore:

- Intelligent network traffic management
- AI-driven QoS optimization
- Adaptive prioritization in distributed systems
- Integration of time-series learning with reinforcement learning
---
## 📌 Future Improvements

- Incorporate real-time packet streaming
- Add attention-based sequence models
- Explore multi-agent reinforcement learning
- Deploy as a live traffic monitoring dashboard
---
## 👨‍💻 Author

Raj Tharani  
B.Tech Computer Science Engineering  
Machine Learning & Systems Research Enthusiast  
---
## ⭐ If you found this interesting

Feel free to star the repository and explore the dataset.
