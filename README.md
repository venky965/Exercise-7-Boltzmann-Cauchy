# Exercise 7: Boltzmann and Cauchy Machines

## Project Title
**Implement Boltzmann and Cauchy Machines for Stochastic Feature Selection and Energy Optimization on the Wine Quality Dataset**

## Objective
To implement a menu-driven stochastic feature selection and energy optimization system using Boltzmann Machine (BM) and Cauchy Machine (CM) models on the Wine Quality dataset.

## Dataset
- **Dataset Name:** Wine Quality (WineQT)
- **File Name:** `WineQT.csv`
- **Target Column:** `quality`
- **Input Features:** Wine chemical properties, such as acidity, residual sugar, chlorides, density, pH, sulphates, and alcohol.

Place `WineQT.csv` in the same directory as the Jupyter Notebook before running the program.

## Technologies Used
- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Methodology

Each feature-selection solution is represented as a binary state vector:

- `1` — Feature selected
- `0` — Feature not selected

The energy function combines classification error with a penalty for selecting more features:

**Energy = Classification Error + Feature Selection Penalty**

Two stochastic optimization methods are implemented:

1. **Boltzmann Annealing:** Uses an energy-based acceptance probability to explore feature subsets.
2. **Cauchy Annealing:** Uses a Cauchy-based acceptance probability to explore alternative feature subsets.

The objective is to find a feature subset with low energy while maintaining classification performance.

## Features

1. Boltzmann Machine Feature Selection
2. Cauchy Machine Feature Selection
3. Comparison of Boltzmann and Cauchy Machines
4. Energy Function Analyzer
5. Random Feature Selection
6. Exit

## Project Structure

```text
Exercise-7-Boltzmann-Cauchy/
├── Exercise_7_Boltzmann_Cauchy.ipynb
├── WineQT.csv
└── README.md
```

## Installation

Install the required Python libraries if they are not already available:

```bash
pip install numpy pandas matplotlib scikit-learn
```

## How to Run

1. Download or obtain the WineQT dataset.
2. Place `WineQT.csv` in the same directory as the notebook.
3. Open `Exercise_7_Boltzmann_Cauchy.ipynb` in Jupyter Notebook.
4. Run the notebook cell containing the complete program.
5. Select an option from the menu.
6. Compare the feature subsets, classification errors, energy values, and optimization graphs.

## Expected Output

The system displays:
- Binary feature-selection vectors
- Selected feature names
- Number of selected features
- Classification accuracy and error
- Energy values
- Boltzmann and Cauchy comparison
- Energy optimization graphs

## Result

The project demonstrates stochastic feature selection using Boltzmann and Cauchy annealing. It compares their ability to search for low-energy feature subsets by considering both classification error and the number of selected features.

## Author
Student Project — Exercise 7
