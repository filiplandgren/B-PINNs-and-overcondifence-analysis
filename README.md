# B-PINNs-and-overcondifence-analysis
Predicting ODEs with limited data and analyzing overconfidence


# BPINN Project

This repository implements a Bayesian Physics-Informed Neural Network (BPINN) for solving differential equations on annular surfaces. It includes training, residual analysis, uncertainty quantification, and PCC analysis.

## Features

* **Data loading** from CSV files
* **Data selection** (random or even sampling)
* **StandardScaler** for preprocessing
* **BayesianPINN** model using Blitz
* **Physics-informed loss** with boundary conditions, turning points, and residuals
* **Training loop** with KL divergence
* **Residual plotting**
* **Uncertainty analysis and validation**
* **PCC analysis** (information density vs. predictive variance)

## Installation

Ensure you have Python 3.7+ and `pip` installed. Then install the required packages:

```bash
pip install torch pandas numpy matplotlib scipy blitz
```

> **Note:** If you have a CUDA-enabled GPU and want GPU acceleration, install the appropriate `torch` package as described on the [PyTorch website](https://pytorch.org/get-started/locally/).

## Usage

1. Place your data CSV files:

   * `DataFirstBranch.csv`
   * `DataSecondBranch.csv`

2. Update the file paths in the script if necessary.


3. The script will train the BPINN on two branches, plot residuals, uncertainty, and conduct PCC analysis.

## File Structure

```
├── README.md
├── bpin_only_model.py          # Main BPINN implementation
├── DataFirstBranch.csv         # Branch 1 data
├── DataSecondBranch.csv        # Branch 2 data
└── requirements.txt            # (Optional) pinned dependencies
```



Requirements:

```
torch
pandas
numpy
matplotlib
scipy
blitz
```

## License

MIT License

---


