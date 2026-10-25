# Neural Networks — Haberman Survival

University project originally developed in 2022 for the **Neural Networks** course and later cleaned and documented for GitHub.

The project applies supervised and unsupervised neural-network techniques to **Haberman's Survival Dataset**, using Python and classic machine-learning libraries.

## Project Overview

The notebook includes:

- loading and exploring the Haberman Survival dataset,
- scatter-matrix and box-plot visualizations,
- missing-value verification,
- MinMax feature scaling,
- feed-forward neural-network classification using Neurolab,
- architecture and training-parameter experiments,
- comparison of different train/test split ratios,
- silhouette-score and elbow analysis,
- competitive neural networks using WTA and CWTA,
- cluster visualization.

## Dataset

The project uses **Haberman's Survival Dataset** from the UCI Machine Learning Repository.

The dataset contains:

- **306 samples**
- **3 input features**
- **2 survival classes**
- **no missing values**

Input features:

1. Age of the patient at the time of operation
2. Year of operation
3. Number of positive axillary nodes detected

Target:

- `1` — patient survived 5 years or longer
- `2` — patient died within 5 years

## Technologies

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- scikit-learn
- Neurolab
- Yellowbrick

## Repository Structure

```text
neural-networks-haberman-survival/
├── data/
│   ├── haberman.data
│   └── haberman.names
├── docs/
│   └── report.md
├── notebooks/
│   └── neural_networks_haberman.ipynb
├── results/
│   ├── plots/
│   └── tables/
├── requirements.txt
└── .gitignore
```

## Main Results

The initial feed-forward neural network used:

- 1 hidden layer
- 5 hidden neurons
- 2 output neurons
- learning rate: `0.3`
- maximum epochs: `3000`
- performance goal: `1e-5`
- resilient backpropagation (RPROP)

The initial 70/30 experiment produced a test accuracy of approximately **71.74%**.

Additional experiments varied:

- number of hidden neurons,
- learning rate,
- number of epochs,
- train/test split ratio.

For unsupervised learning, silhouette analysis selected **2 clusters**, which was then used for competitive-network experiments with WTA and CWTA.

## Running the Project

Create a Python environment and install the dependencies:

```bash
python -m pip install -r requirements.txt
```

Then open:

```text
notebooks/neural_networks_haberman.ipynb
```

and run the notebook from the beginning.

## Notes

This repository keeps the scope and methodology of the original university project while correcting implementation and reproducibility issues found in the original 2022 notebook.

It is intentionally presented as a university Neural Networks project rather than being converted into a modern deep-learning implementation.

## Documentation

A more detailed description of the methodology and results is available in:

```text
docs/report.md
```
