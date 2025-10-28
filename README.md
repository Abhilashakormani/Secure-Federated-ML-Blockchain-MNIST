# Secure-Federated-ML-Blockchain-MNIST

Secure Collaborative Machine Learning using Federated Learning and Blockchain on MNIST Dataset

## Introduction

This project implements a secure collaborative machine learning system that combines federated learning with blockchain technology to train models on the MNIST dataset. The system enables multiple parties to collaboratively train a machine learning model without sharing their raw data, ensuring privacy and security. Blockchain technology is utilized to maintain transparency, immutability, and trust in the federated learning process by recording model updates and ensuring the integrity of the training process.

## System Architecture

The system architecture consists of the following key components:

- **Federated Learning Framework**: Enables distributed model training across multiple clients without centralized data collection
- **Blockchain Network**: Maintains a decentralized ledger of model updates and training metrics
- **MNIST Dataset**: Handwritten digit recognition dataset distributed across participating nodes
- **Central Aggregator**: Coordinates the federated learning rounds and aggregates local model updates
- **Smart Contracts**: Automate verification and validation of model updates on the blockchain
- **Client Nodes**: Individual participants that train local models on their private MNIST data subsets

## Tools & Libraries

- **Python 3.8+**: Primary programming language
- **TensorFlow/Keras**: Deep learning framework for model development
- **PySyft**: Privacy-preserving machine learning library for federated learning
- **Web3.py**: Python library for blockchain interaction
- **Ethereum/Ganache**: Blockchain platform for decentralized ledger
- **Solidity**: Smart contract development language
- **NumPy**: Numerical computing library
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Visualization library for results

## Setup Instructions

### Prerequisites
- Python 3.8 or higher
- Node.js and npm (for blockchain development)
- Git

### Installation Steps

1. Clone the repository:
```bash
git clone https://github.com/Abhilashakormani/Secure-Federated-ML-Blockchain-MNIST.git
cd Secure-Federated-ML-Blockchain-MNIST
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required dependencies:
```bash
pip install tensorflow syft web3 numpy pandas matplotlib
```

4. Set up the blockchain environment:
```bash
npm install -g ganache-cli
ganache-cli
```

5. Deploy smart contracts (in a new terminal):
```bash
python deploy_contracts.py
```

6. Run the federated learning system:
```bash
python main.py
```

### Configuration

- Configure the number of client nodes in `config.py`
- Adjust blockchain network settings in `blockchain_config.json`
- Modify model hyperparameters in `model_config.py`

---

*This project demonstrates the integration of federated learning and blockchain technology for secure and transparent collaborative machine learning.*
