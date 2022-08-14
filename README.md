# DeepRL-for-Portfolio-Management

The notebook contains the application of various Deep Reinforcement Learning algorithms to the problem of managing a financial portfolio with the objective maximize the return. The tested algorithms are:
- Advantage Actor-Critic (A2C)
- Proximal Policy Optimization (PPO)
- Twin Delayed Deep Deterministic Policy Gradients (TD3)

The universe in which the agent can pick assets is composed of Italian blue chip stocks (part of the FTSE MIB index) and cash. The environment constrains the agent to be long-only and includes transaction costs. The final results on the testing set, from January 2019 to March 2021, show a significant outperformance:
Algorithm     | Returns | Sharpe Ratio
------------- | ------- | ------------
FTSE MIB ETF  | 38.58%  | 1.06
A2C           | 48.36%  | 1.24
PPO           | 48.47%  | 1.22
TD3           | 45.70%  | 1.17
