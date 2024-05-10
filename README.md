# VGAE-Cora-Workout

## Overview
This repository contains an implementation of Graph Autoencoder (GAE) and Variational Graph Autoencoder (VGAE) models for learning latent representations of graphs. These models are designed to capture the underlying structure of graph data, making them suitable for a wide range of applications in graph analytics, including node classification, link prediction, and community detection.

## Features
- **GAE and VGAE Models**: Implementations of both GAE and VGAE models, providing flexibility in choosing between deterministic and probabilistic latent representations.
- **Graph Convolutional Layers**: Graph convolutional layers are used as building blocks for encoding node features and capturing graph structure.
- **Variational Inference**: VGAE incorporates variational inference techniques to learn probabilistic latent representations, enabling uncertainty estimation and robustness to noise.
- **Preprocessing Utilities**: Preprocessing functions for loading and preprocessing graph data, including adjacency matrix normalization and test set generation.
- **Training and Evaluation**: Training loop with support for monitoring training loss, validation scores (ROC and Average Precision), and evaluation on a held-out test set.

## Dependencies
- Python 3
- PyTorch
- NetworkX
- SciPy
- NumPy
- Scikit-learn

## Usage
1. **Data Preparation**: Prepare your graph data in the required format. The dataset should include the adjacency matrix and node features.
2. **Configuration**: Adjust the configuration parameters in the `args.py` file to specify the dataset, model type (GAE or VGAE), and training hyperparameters.
3. **Training**: Run the training script (`train.py`) to train the chosen model on your dataset. Monitor training progress and validation scores to assess model performance.
4. **Evaluation**: After training completes, evaluate the trained model on a held-out test set to assess its generalization performance.
5. **Analysis**: Analyze the learned latent representations and reconstructed adjacency matrix to gain insights into the underlying graph structure.

## Credits
The implementation is inspired by the work of Thomas Kipf and his paper on graph autoencoders and Github Repo (https://github.com/DaehanKim/vgae_pytorch). Preprocessing functions are adapted from Kipf's implementation for consistency with commonly used datasets.

## License
This project is licensed under the GPL License.
