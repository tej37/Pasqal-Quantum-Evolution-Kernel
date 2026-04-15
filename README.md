# ⚛️ Pasqal Quantum Evolution Kernel (QEK)

This project reproduces the official Pasqal tutorial on the **Quantum Evolution Kernel (QEK)** — a quantum-inspired approach to machine learning on graph data.

🔗 Tutorial: https://docs.pasqal.com/applicationsolvingtools/qek/

---

## 📌 Overview

The **Quantum Evolution Kernel (QEK)** is an open-source Python library designed to compute similarity between graph-structured data using quantum-inspired techniques.

It enables the integration of quantum concepts into classical machine learning workflows, particularly for tasks like classification using kernel methods.

In this project, I reproduced the tutorial demonstrating how to:
- Extract quantum-inspired features from graph data
- Build a custom kernel based on quantum evolution
- Train a machine learning model (SVM)
- Evaluate its performance

This is a **hybrid quantum-classical approach**, combining quantum feature extraction with classical ML models.

---

## 🧠 Key Concept

The Quantum Evolution Kernel is defined as:

\[
K(G, G') = \exp \left( -\mu \cdot JS(P_G, P_{G'}) \right)
\]

Where:
- \( G, G' \): graphs
- \( P_G \): excitation distribution of graph \( G \)
- \( JS \): Jensen-Shannon divergence
- \( \mu \): hyperparameter controlling similarity

---

## ⚙️ Workflow

### 1. Data Preparation
- Load graph dataset (molecular data)
- Extract features (quantum excitation distributions)

### 2. Kernel Construction
- Use `FastQEK` for efficient computation
- Fit kernel on training data
- Transform data into kernel matrices

### 3. Model Training
- Train a Support Vector Machine (SVM) using the QEK kernel

### 4. Evaluation
- Evaluate model performance using:
  - F1 Score
  - Balanced Accuracy

---

## 🛠️ Technologies

- Python
- qek (Quantum Evolution Kernel library)
- scikit-learn
- NumPy

---

## dependencies
$ pip install quantum-evolution-kernel
or
$ pipx install quantum-evolution-kernel
