# RIVAL: Breaking Spurious Correlations in Smart Contract Vulnerability Detection

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
[![PyTorch 1.12+](https://img.shields.io/badge/PyTorch-1.12+-ee4c2c.svg)](https://pytorch.org/)

This is the official implementation of **RIVAL**, a robust invariant representation learning framework designed to mitigate spurious correlations in smart contract vulnerability detection.

---

## 📖 Overview

Deep learning models for vulnerability detection often suffer from **spurious correlations**—relying on non-essential features (e.g., variable naming styles) rather than core vulnerability logic. **RIVAL** addresses this via a two-stage causal intervention strategy:
1. **Stage I (Robust Pre-training):** Enforces causal invariant learning across semantically perturbed domains using cross-domain alignment and context-aware masking.
2. **Stage II (Downstream Classification):** Transfers the artifact-free encoder for precise vulnerability detection across multiple contract types.

### 🏗️ Architecture
![Architecture](figures/architecture.png) **

---

## 🛠️ Installation

### Prerequisites
- Linux Server (Tested on Ubuntu 20.04)
- Python 3.7+
- NVIDIA GPU (RTX 3090 or higher recommended) + CUDA 11.x

### Setup
```bash
# Clone the repository
git clone [https://github.com/](https://github.com/)[YourUsername]/RIVAL.git
cd RIVAL

# Create a virtual environment
conda create -n rival python=3.7
conda activate rival

# Install dependencies
pip install -r requirements.txt
