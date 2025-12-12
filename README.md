# Deep Reinforcement Learning for Stock Trading

This project applies deep reinforcement learning to stock trading using **PPO, A2C, and Double DQN** agents on historical stock price data downloaded from Yahoo Finance. The goal is to learn a trading policy that outperforms a simple buy-and-hold baseline while controlling risk.

## Project structure

- `PPO-A2C-Stock-trading-project.ipynb` – main end-to-end notebook:
  - Data download and preprocessing
  - Custom trading environment
  - Training PPO and A2C agents
  - Evaluation and performance plots

- `stock-market-double-dqn.ipynb` – Double DQN experiment on the same or similar trading environment.

- `experiments/upgraded-2yrs-yahoo-data.ipynb` – extended training on two years of historical stock data.

- `experiments/Testing-Google-n-Walmart.ipynb` and `experiments/Testing-IBM-n-GE.ipynb` – additional backtests on different ticker combinations.

## Environment and actions

- **State**: sliding window of recent OHLCV/feature data (exact details are defined in the main notebook).
- **Actions**: discrete actions such as **Buy**, **Hold**, and **Sell**.
- **Reward**: change in portfolio value (including unrealized PnL) at each time step, optionally including transaction costs.

## How to run

1. Clone the repo:

```bash
git clone https://github.com/Sailaja-ASB/Deep-RL-Stock-Trading.git
cd Deep-RL-Stock-Trading
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the main notebook in Jupyter:

```bash
jupyter notebook PPO-A2C-Stock-trading-project.ipynb
```

## Future work

- Add Dueling or Rainbow DQN.
- Extend to multi-asset portfolio optimization.
- Model realistic transaction costs and slippage.

👩‍💻 Author

Sailaja Morrennagari /n
GitHub: https://github.com/Sailaja-ASB /n
LinkedIn: https://www.linkedin.com/in/sailajamorrennagari
