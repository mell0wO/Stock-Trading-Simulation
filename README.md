# Stock Trading Simulation

## Overview
This project, developed as part of a DataCamp course, focuses on implementing a reinforcement learning (RL) simulation for stock trading in Python. It is designed under the fictional trading firm **Quantum Trading**, which aims to leverage machine learning for financial market advantages.

Traditional trading strategies often rely on historical data and predefined rules that may not adapt quickly to changing market conditions. Reinforcement learning, a branch of machine learning where an agent learns by interacting with its environment, presents a promising alternative. By using RL, trading algorithms can learn and adapt in real-time, improving their performance over time.

## Features
- Implements reinforcement learning using **Stable-Baselines3 PPO (Proximal Policy Optimization)**
- Uses **Gymnasium and gym_anytrading** for market simulation
- Trains an RL agent to buy and sell stocks dynamically
- Evaluates trading performance with **balance tracking and visualization**
- Works with **historical stock data (AAPL.csv)**

## Installation
To run this project, you need to have Python installed. Follow the steps below:

```sh
# Clone the repository
git clone https://github.com/mell0wO/Stock-Trading-Simulation
cd Stock-Trading-Simulation

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Dataset
The project uses **AAPL.csv**, which contains historical prices for Apple Inc. The dataset includes:

| Column | Description |
|--------|-------------|
| Date   | The date corresponding to the closing price |
| Close  | The closing price of the stock on the given date |

## How It Works
1. Load historical stock data
2. Create a trading environment using **Gym's 'stocks-v0'**
3. Train an RL agent using **Stable-Baselines3 PPO**
4. Simulate trading decisions and track performance
5. Visualize **trading actions and balance history**

## Output Example
- **Observation Space:** Box(-10000000000.0, 10000000000.0, (10, 2), float32)
- **Training Metrics:**
  - Iterations: 1
  - Total Timesteps: 2048
  - Policy Loss, Value Loss, Approx KL, etc.
- **Trading Actions:**
  - Buy/Sell signals and balance updates
  - Debug logs for decisions taken
- **Final Balance:** $566,773.55 (Example Output)

## Visualizations
- **Trading Actions Plot:** Stock price with buy/sell markers
- **Balance History Plot:** Tracks changes in balance over time

## Technologies Used
- **Python**
- **Gymnasium & gym_anytrading**
- **Stable-Baselines3 (PPO Algorithm)**
- **Matplotlib & Pandas**
- **NumPy**

## Disclaimer
**This project is for educational purposes only. It is not financial advice and should not be understood as such. Use at your own risk.**

## License
This project is licensed under the MIT License. See `LICENSE` for details.

## Contributing
**Contributions are welcome! Feel free to submit a pull request or report any issues.
**---

Happy Trading 🚀
