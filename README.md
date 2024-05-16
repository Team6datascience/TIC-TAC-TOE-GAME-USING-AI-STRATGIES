# TIC-TAC-TOE-GAME-USING-AI-STRATGIES  USER MANUAL
# How to Use the Code:

## 1. Running the Code:

Open the code file in your preferred Python environment (e.g., Jupyter Notebook, Python IDE).
To run this script without any compatibility issues, it is recommended to use one of the following Python versions:

Python 3.6,
Python 3.7,
Python 3.8,
Python 3.9,
Python 3.10,
Python 3.11.
If you are using Google Colab, it typically runs Python 3.8 or 3.9, which should be perfectly suitable for this script.
Execute the code cell or run the script to start the simulations.

Required Python Packages:

Jupyter Notebook: To run the notebook.
matplotlib: For plotting the training progress.
numpy: For numerical operations.
IPython: For the clear_output function, which helps clear the output in the notebook.

Customization:

You can customize the parameters of the simulations to suit your needs:
Adjust the num_simulations variable to change the number of games played in each simulation.
Modify the num_runs variable to control the number of times the simulations are repeated.
Tune the parameters of the Q-learning and MCMC players (e.g., epsilon, alpha, gamma for Q-learning; num_simulations for MCMC) to experiment with different learning strategies.

## 2. Understanding the Results:

Simulation Results:

After running the simulations, the code will print the following information:
Number of wins for the Q-learning player.
Number of wins for the MCMC player.
Number of tie games.
These results provide insights into the performance of both players and the competitiveness of the games.
Average Win Rates:
Additionally, the code calculates and prints the average win rates for both players.
The average win rate is the total number of wins divided by the total number of simulations or runs.
This metric helps gauge the overall effectiveness of each player's strategy across multiple games.

## 3. Interpreting the Bar Chart:

### Visualization:
The code generates a bar chart to visually represent the average win rates of the Q-learning and MCMC players.
The x-axis shows the player types (Q-learning, MCMC) and tie games.
The y-axis indicates the average number of wins.
Each bar represents the average win count for a specific player or tie game.
### Comparison:
Users can compare the heights of the bars to assess the relative performance of the Q-learning and MCMC players.
A higher bar indicates a higher average win rate, suggesting a more successful strategy.

## 4. Understanding the Players:

### QLearningPlayer:
This player implements the Q-learning algorithm, a model-free reinforcement learning technique, to learn optimal strategies through trial and error.
### Parameters:
epsilon: Controls the exploration-exploitation trade-off by determining the probability of choosing a random action versus the best action.
alpha: Governs the learning rate, influencing the extent to which Q-values are updated based on new information.
gamma: Represents the discount factor, indicating the importance of future rewards in the learning process.

### MCMCPlayer:

This player utilizes Monte Carlo simulations to estimate win probabilities for potential moves and selects the move with the highest estimated probability.

### Parameters:

num_simulations: Specifies the number of simulations to run for estimating win probabilities. Higher values may yield more accurate estimates but require more computation.

## 5. Interpreting the Tic-Tac-Toe Game:

### Game Mechanics:
The Tic-Tac-Toe game follows standard rules, where two players (AI_PLAYER_1 and AI_PLAYER_2) take turns placing their markers (X or O) on a 3x3 grid.
The game ends when one player achieves a winning sequence (three consecutive markers in a row, column, or diagonal) or when the board is full (resulting in a tie).

### Game Outcome:
After each game, the code determines the winner or declares a tie based on the final board configuration.
The number of wins for each player is tallied to evaluate their performance over multiple games.

## 6. Tuning Parameters:

### Experimentation:
Users can experiment with different parameter values to observe their effects on the players' performance and learning behavior.
Adjusting parameters such as epsilon, alpha, gamma, and num_simulations allows for fine-tuning the players' strategies and learning dynamics.
