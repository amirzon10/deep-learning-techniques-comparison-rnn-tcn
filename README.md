# Deep Learning Techniques Comparison (RNN vs ResNet) — TensorFlow vs PyTorch

Repository for an Applied Deep Learning group project. It contains shared preprocessing logic, two deep learning techniques implemented in two frameworks (TensorFlow and PyTorch), saved model weights, intermediate results, and artefacts used to answer two research questions around reproducibility and dataset effects. [page:1]

## Project context (CA brief)

This project builds a small *portfolio* of deep learning methods to answer two research questions:

- **RQ1 (Reproducibility across implementations):** Do identically-named deep learning techniques perform the same across different implementations (e.g., TensorFlow vs PyTorch) when evaluated under identical empirical conditions?
- **RQ2 (Dataset characteristics):** How do datasets differ, and how do these differences affect model performance? This includes analysing dataset characteristics such as variable types, record counts, summary statistics, cleaning steps, normalization, balancing, and train/test splits.

The goal is to demonstrate consistent experimental design, fair comparisons, and clear explanation of why results differ (implementation details, training dynamics, preprocessing mismatches, etc.).

## What’s in this repo

At the time of writing, the `main` branch includes: [page:1]

- Two notebooks:
  - `Tensorflow_implementation.ipynb` [page:1]
  - `Pytorch_implementation.ipynb` [page:1]
- Saved best model weights in both ecosystems (`.pth` for PyTorch and `.weights.h5` for TensorFlow). [page:1]

> Note: The repo name suggests RNN / TCN / ResNet, but the visible artefacts in `main` currently show RNN and ResNet weights/notebooks. If TCN is part of the final submission, add it to the README sections below once merged. [page:1]

## Branches and ownership

This repository uses a simple branch-per-owner workflow, where the `main` branch is Amir’s primary branch and other active branches are named after their respective owners. [page:2]

- `main` (default) — Amir’s main branch and the canonical integration branch. [page:2]
- `Deepak` — Deepak’s working branch. [page:2]
- `Semin` — Semin’s working branch. [page:2]

## How to run (high level)

The project is notebook-driven. Start by opening one of the notebooks and running cells top-to-bottom:

- TensorFlow pipeline: `Tensorflow_implementation.ipynb` [page:1]
- PyTorch pipeline: `Pytorch_implementation.ipynb` [page:1]

Ensure both implementations use identical dataset splits, identical preprocessing/normalization, and comparable training/evaluation settings to keep the RQ1 comparison valid.

## Artefacts

Trained model checkpoints are stored in-repo for reproducibility and comparison: [page:1]

- PyTorch weights: e.g., `best_rnn_model.pth`, `best_resnet.pth`, `best_power_resnet.pth`, `best_power_RNN.pth` [page:1]
- TensorFlow weights: e.g., `best_rnn_model.weights.h5`, `best_resnet.weights.h5`, `best_power_resnet.weights.h5`, `best_power_RNN..weights.h5` [page:1]

## Contributor notes

### Deepak

- **Datasets:** Dataset 1 (HAR), Dataset 2 (Bike Sharing)
- **Techniques:** Vanilla RNN, TCN
- **Implementations:** RNN (TensorFlow), RNN (PyTorch), TCN (TensorFlow), TCN (PyTorch)

### Amir (main)

- **Datasets:** Dataset 2 (Bike Sharing), Dataset 3 (Household Power Consumption)
- **Techniques:** Vanilla RNN, ResNet
- **Implementations:** RNN (TensorFlow), RNN (PyTorch), TCN (TensorFlow), TCN (PyTorch)

### Semin

- **Datasets:** Dataset 1 (HAR), Dataset 3 (Household Power Consumption)
- **Techniques:** ResNet, TCN
- **Implementations:** RNN (TensorFlow), RNN (PyTorch), TCN (TensorFlow), TCN (PyTorch)
(TODO)

## License / academic integrity

This is a course project repository. Reuse or redistribution should follow the course’s academic integrity requirements and any dataset licensing constraints.
