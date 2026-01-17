# 🎲 The Monte Carlo Minesweeper

**[Play Now](https://minesweeper.otischan.dev/)** ⚡

An advanced Minesweeper implementation featuring **Monte Carlo probability calculations** and **entropy-based optimal move analysis**. A strategic decision-making tool powered by probability theory and information theory.

## ✨ Features

- **Monte Carlo Simulation**: Calculate precise survival probabilities using constraint satisfaction algorithms
- **Entropy Analysis**: Identify optimal moves based on expected information gain
- **Real-time Visualization**: Probability percentages and entropy values overlaid on the board
- **AI-Powered Recommendations**: Intelligent suggestions for the best strategic moves
- **Chord Clicking**: Advanced gameplay mechanics for experienced players

## 📁 Project Structure

```
montecarlo_entropy_minesweeper/
├── index.html          # Main game file (HTML + CSS + JS)
└── README.md           # This file
```

## 🧮 Monte Carlo Algorithm

The probability calculator uses a backtracking algorithm to enumerate valid mine configurations that satisfy all visible constraints (revealed numbers). Each configuration is weighted using binomial coefficients to account for interior cell arrangements, providing accurate probability estimates.

## 🧠 Entropy Calculation

Expected information gain is calculated using:
- **Shannon entropy** for cells with uncertain mine probability
- **Constraint counting** for frontier cells (adjacent to revealed numbers)
- **Neighbor analysis** to predict information cascade potential

The scoring function balances:
```
Score = (Survival Probability) × (Expected Information Gain)
```

This ensures recommendations prioritize both safety and strategic value.
