# 🧠 SVM Optimization on UCI Letter Recognition Dataset

This project focuses on optimizing a **Support Vector Machine (SVM)** classifier on the UCI **Letter Recognition Dataset**. The goal is to maximize classification accuracy across 10 different random samples using parameter tuning.

---

## 📊 Dataset Overview

- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/letter+recognition)
- **Type:** Multi-class classification (26 classes: A-Z)
- **Size Used:** 5,000 rows (random subset)

---

## 🧪 Project Steps

1. 🔽 **Load and clean** dataset  
2. 🔄 **Split** data into 10 different 70/30 train-test samples  
3. 🔧 **Optimize SVM** parameters:
   - Kernel type: `rbf`, `linear`
   - Regularization `C`: 0.1, 1, 10
   - 20 random parameter combinations per sample  
4. 📈 **Track accuracy** over iterations  
5. 🥇 **Log best parameters** and **plot convergence graph** for best-performing sample

---

## 📌 Results Summary

| Sample | Best Accuracy | Kernel | C  |
|--------|----------------|--------|----|
| S1     | 0.9240         | rbf    | 10 |
| S2     | 0.9247         | rbf    | 10 |
| S3     | 0.9340         | rbf    | 10 |
| S4     | 0.9280         | rbf    | 10 |
| S5     | **0.9413**     | rbf    | 10 |
| S6     | 0.9240         | rbf    | 10 |
| S7     | 0.9340         | rbf    | 10 |
| S8     | 0.9253         | rbf    | 10 |
| S9     | 0.9153         | rbf    | 10 |
| S10    | 0.9340         | rbf    | 10 |

✅ Best accuracy achieved: **94.13% (S5)**

---

## 📊 Convergence Plot (S5)

![Convergence](convergence_best_sample.png)

---

## 🛠️ Tech Stack

- Python
- scikit-learn
- pandas, numpy
- matplotlib, seaborn

---

## 💾 How to Run

```bash
pip install -r requirements.txt
python svm_optimizer.py
