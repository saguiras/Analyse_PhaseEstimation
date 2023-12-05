

# Analyse Phase Estimation
Ce module Python utilise Q# et Jupyter Notebooks pour effectuer une analyse approfondie de l'estimation de phase quantique. L'objectif principal est de comprendre le comportement de l'erreur d'estimation en fonction du nombre de tirs (n_shots) et du nombre d'oracles (n_oracle), en appliquant la Loi des Grands Nombres.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/saguiras/Analyse_PhaseEstimation.git
    cd Analyse_PhaseEstimation
    ```

2. Environment setup:
    ```bash
    pip install qsharp 
    ```
    ```bash
    dotnet tool install -g Microsoft.Quantum.IQSharp
    ```
    ```bash
    dotnet iqsharp install
    ```
    ```bash
    pip install -r requirements.txt
    ```
    

## Usage

The main functionality of this module is encapsulated in the `find_best_parameter` function. To use it in your code, you can follow these steps:

```python
num_simulations = 10
n_shot_values_combined = list(range(1, 15))
n_oracle_values_combined = list(range(1, 35))

best_values_combined, avg_phi_diff_combined = find_best_parameter(
   n_shot_values_combined , n_oracle_values_combined, num_simulations
)
```
