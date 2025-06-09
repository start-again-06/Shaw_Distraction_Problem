# Shaw_Distraction_Problem

# 📊 Singular Value Decomposition (SVD) Analysis 🔢

## 🔍 Overview
This project explores numerical computations using **Singular Value Decomposition (SVD)** and matrix transformations. The code performs **discretization**, **filtering**, and **inverse problem regularization** to analyze system behavior in ill-conditioned settings.

---

## ✨ Features
✅ **Matrix Transformation** – Generates weight matrix `G` using trigonometric functions  
✅ **Singular Value Decomposition (SVD)** – Decomposes `G` into its principal components (`U`, `S`, `V`)  
✅ **Regularization Parameter Tuning** – Computes stabilized solutions using Tikhonov-like filtering  
✅ **Log-Log Plot Analysis** – Visualizes error vs. solution norm to evaluate stability

---

## 🛠 Installation
Ensure you have **MATLAB** or **GNU Octave** installed to run this script.

---

## 📑 Computation Breakdown

### 1️⃣ Weight Matrix (G) Construction
- Constructs transformation matrix `G` using trigonometric operations  
- Handles potential **singularities** in function evaluations  

### 2️⃣ Singular Value Decomposition (SVD) Analysis
- Performs SVD on matrix `G`:  
  \[
  G = U \cdot S \cdot V^T
  \]  
- Analyzes **rank**, **condition number**, and **singular values**

### 3️⃣ Regularization Parameter (α) Optimization
- Iteratively computes **filtered solutions** across a range of `α` values  
- Applies filtering function:  
  \[
  f(i) = \frac{s(i)^2}{s(i)^2 + \alpha(j)^2}
  \]  
- Balances **solution stability** and **accuracy**

### 4️⃣ Visualization & Analysis
- **Stair-step plots** show filtered transformation results  
- **Log-log plots** reveal tradeoff between reconstruction error and solution norm

---

## 📊 Results & Insights
- **Singular values** dictate numerical sensitivity and inversion robustness  
- **Tikhonov regularization** filters unstable components from small singular values  
- **Log-log analysis** identifies the optimal α for minimal error and acceptable norm

---

## 🔚 Conclusion
This project demonstrates how **SVD-based filtering** improves **numerical stability** in solving **inverse problems**. It provides a structured approach for **analyzing and regularizing ill-conditioned systems** using mathematical rigor and visual validation.

---

## 📜 License

🔓 **MIT License** – Free to use and modify!

