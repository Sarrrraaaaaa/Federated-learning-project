# Federated Learning Project

This repository demonstrates two approaches to federated learning using a diabetes dataset: horizontal federated learning and vertical federated learning.

## Repository Structure

- [`diabetes.csv`](diabetes.csv): The dataset used for training and evaluation.
- [`horizintal_fl.py`](horizintal_fl.py): Implementation of horizontal federated learning, including integration with a smart contract for client consent management using Web3.
- [`vertical_fl.py`](vertical_fl.py): Implementation of vertical federated learning, where each client holds different features of the same patients.
- [`README.md`](README.md): Project documentation.

## Requirements

- Python 3.7+
- TensorFlow
- TensorFlow Federated
- scikit-learn
- pandas
- numpy
- web3 (for horizontal FL)
- Ganache or an Ethereum-compatible endpoint (for horizontal FL)

## Usage

### 1. Horizontal Federated Learning

This script simulates federated learning where each client has a subset of the data (same features, different samples). It integrates a consent mechanism based on an Ethereum smart contract.

Run:
```sh
python horizintal_fl.py
```

### 2. Vertical Federated Learning

This script simulates federated learning where each client has different features for the same patients.

Run:
```sh
python vertical_fl.py
```

## Dataset

The [`diabetes.csv`](diabetes.csv) file contains medical features of patients and the `Outcome` column indicating diabetes presence (1) or absence (0).

## Notes

- You may need to adjust file paths depending on your environment.
- For horizontal FL, ensure you have access to an Ethereum endpoint (Ganache, Infura, etc.) and update the contract address and ABI as needed.

## Authors

Project created as a demonstration of federated
