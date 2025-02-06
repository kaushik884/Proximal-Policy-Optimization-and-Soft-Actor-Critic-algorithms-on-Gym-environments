# Comparative Analysis of Soft Actor-Critic (SAC) and Proximal Policy Optimization (PPO) Algorithms

This project investigates and compares the performance of two reinforcement learning (RL) algorithms: **Soft Actor-Critic (SAC)** and **Proximal Policy Optimization (PPO)**. The study was conducted across three distinct OpenAI Gym environments: **Taxi-v3**, **CartPole-v1**, and **LunarLander-v2**, representing grid-based navigation, dynamic balancing, and precision control tasks respectively.

## Project Objectives
- Analyze and compare SAC and PPO algorithms across discrete and continuous environments.
- Evaluate performance metrics such as cumulative rewards, training stability, and convergence speed.
- Identify the strengths and weaknesses of each algorithm for different types of RL tasks.

## Environments
1. **Taxi-v3**  
   A grid-based discrete task where the agent controls a taxi to pick up and drop off passengers at specific locations.
   
2. **CartPole-v1**  
   A continuous balancing task where the agent applies forces to a cart to keep a pole balanced upright.

3. **LunarLander-v2**  
   A hybrid control task requiring the agent to control a lander’s orientation and thrust to achieve a safe landing on a designated pad.

## Algorithms
### Soft Actor-Critic (SAC)
- **Type**: Off-policy  
- **Key Features**:
  - Entropy regularization to encourage exploration.
  - Stochastic policy with dual Q-networks to reduce overestimation bias.
  - Designed for continuous control tasks with gradual, stable learning.

### Proximal Policy Optimization (PPO)
- **Type**: On-policy  
- **Key Features**:
  - Policy clipping to ensure stability and limit large updates.
  - Suitable for both discrete and continuous environments.
  - Rapid early learning with effective exploration-exploitation balance.

## Project Phases
### 1. Environment Setup and Agent Development
- Integrated OpenAI Gym environments.
- Implemented SAC and PPO agents tailored to each task.

### 2. Training and Performance Evaluation
- Measured performance based on:
  - **Cumulative Rewards**: Total rewards achieved per episode.
  - **Training Stability**: Reward fluctuations and convergence behavior.
  - **Learning Efficiency**: Speed of performance improvements during training.

### 3. Data Collection and Analysis
- Collected training data and visualized performance using reward plots.
- Conducted a detailed comparison of SAC and PPO in various scenarios.

## Results Summary
- **SAC**: 
  - Performed better in complex environments (e.g., LunarLander).
  - Demonstrated stable long-term performance with fewer reward fluctuations.
  
- **PPO**: 
  - Achieved faster learning in simpler environments (e.g., CartPole).
  - Less stable in complex scenarios, with notable reward fluctuations.

## Technologies Used
- **Python**: Algorithm development and data analysis.
- **OpenAI Gym**: Simulation environments for RL tasks.
- **Matplotlib**: Visualization of training progress.
- **RL Libraries**: Implementations of SAC and PPO for benchmarking.

## Key Learnings
- SAC is better suited for complex, continuous control tasks requiring stability and exploration.
- PPO excels in simpler, discrete tasks with faster convergence but lower long-term stability.
- Task complexity and action space characteristics are critical when selecting RL algorithms for real-world applications.

## Future Work
- Evaluate these algorithms in more diverse or real-world environments.
- Explore additional metrics such as computational efficiency and robustness to hyperparameter changes.
- Investigate scalability to higher-dimensional tasks.

## References
- OpenAI Gym Documentation: [https://gymnasium.farama.org/](https://gymnasium.farama.org/)
- Spinning Up RL Documentation: [https://spinningup.openai.com/](https://spinningup.openai.com/)

For more details and code implementation, visit the project repository: [GitHub Link](https://github.com/kaushik884/RLProject)
