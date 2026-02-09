# 🧠 K-Means Clustering Implementation from Scratch

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://python.org)
[![NumPy](https://img.shields.io/badge/NumPy-1.21%2B-013243?logo=numpy&logoColor=white)](https://numpy.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Code Size](https://img.shields.io/github/languages/code-size/your-username/kmeans-from-scratch)](https://github.com/your-username/kmeans-from-scratch)

> A complete implementation of the K-Means clustering algorithm from scratch using pure NumPy, with comprehensive comparison against scikit-learn's optimized implementation. Includes elbow method analysis for optimal cluster selection and professional visualizations.

![K-Means Clustering Visualization](https://via.placeholder.com/800x400/e0e0e0/000000?text=Cluster+Visualization+Preview)

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [✨ Key Features](#-key-features)
- [⚙️ Installation](#-installation)
- [🚀 Quick Start](#-quick-start)
- [🔬 Methodology](#-methodology)
- [📊 Results & Visualizations](#-results--visualizations)
- [📁 Project Structure](#-project-structure)
- [📐 Elbow Method Explained](#-elbow-method-explained)
- [⚖️ Custom vs scikit-learn Comparison](#-custom-vs-scikit-learn-comparison)
- [📚 References](#-references)
- [📄 License](#-license)

## 📌 Project Overview

This project demonstrates a **from-scratch implementation** of the K-Means clustering algorithm using only NumPy—without relying on scikit-learn's clustering module for the core algorithm. The implementation follows Lloyd's algorithm and includes:

- ✅ Random centroid initialization
- ✅ Iterative assignment and update steps using Euclidean distance
- ✅ Convergence detection with tolerance-based stopping criteria
- ✅ Inertia calculation (within-cluster sum of squares)
- ✅ Elbow method analysis to determine optimal cluster count (`k`)
- ✅ Side-by-side comparison with scikit-learn's production implementation
- ✅ Comprehensive visualizations of clusters, centroids, and evaluation metrics

Designed primarily as an **educational resource**, this project bridges the gap between theoretical understanding and practical implementation of one of machine learning's most fundamental unsupervised algorithms.

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| **Pure NumPy Implementation** | Core algorithm built entirely with NumPy—no external clustering libraries used |
| **Elbow Method Analysis** | Automatic identification of optimal `k` through inertia visualization (k=2 to k=7) |
| **Dual Implementation Comparison** | Side-by-side results showing near-identical output between custom and scikit-learn versions |
| **Reproducible Results** | Fixed random seeds (`random_state=42`) ensure consistent outputs across runs |
| **Synthetic Dataset Generation** | Uses `make_blobs` to create clean 2D clusters with configurable parameters |
| **Professional Visualizations** | Matplotlib plots with labeled centroids, color-coded clusters, and informative titles |
| **Quantitative Metrics** | Console output showing inertia values and centroid coordinates for direct comparison |

## ⚙️ Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup Instructions
```bash
# Clone the repository
git clone https://github.com/your-username/kmeans-from-scratch.git
cd kmeans-from-scratch

# Create and activate virtual environment (recommended)
python -m venv venv
source venv/bin/activate          # Linux/MacOS
# OR
venv\Scripts\activate             # Windows

# Install dependencies
pip install -r requirements.txt
