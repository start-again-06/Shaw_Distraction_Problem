# Shaw_Distraction_Problem

📊 Singular Value Decomposition (SVD) Analysis 🔢
🔍 Overview
This project explores numerical computations using Singular Value Decomposition (SVD) and matrix transformations. The code performs discretization, filtering, and inverse problem regularization to analyze system behavior.

✨ Features
✅ Matrix Transformation – Generates weight matrix G using trigonometric functions
✅ Singular Value Decomposition (SVD) – Decomposes G into its principal components
✅ Regularization Parameter Tuning – Computes stabilized solutions using Tikhonov-like filtering
✅ Log-Log Plot Analysis – Evaluates error vs. solution norm

🛠 Installation
Ensure you have MATLAB or GNU Octave installed to run this script.

📑 Computation Breakdown
1️⃣ Weight Matrix (G) Construction

Computes transformation weights using trigonometric functions
Handles singularities in function evaluation
2️⃣ Singular Value Decomposition (SVD) Analysis

Decomposes matrix G into U, S, V
Determines the rank of G
3️⃣ Regularization Parameter (α) Optimization

Computes a series of filtered solutions
Balances stability vs. accuracy
4️⃣ Visualization & Analysis

Stair-step plot to inspect transformation output
Log-log plot for error vs. solution magnitude
📊 Results & Insights
Singular values determine the numerical stability of the system.
Regularization smooths the solution by filtering unstable components.
Log-log curve provides insights into error behavior and solution stability.
🔚 Conclusion
This analysis demonstrates how SVD-based filtering improves numerical stability in inverse problems. It provides a structured approach to solving ill-conditioned systems with regularization techniques.

📜 License
🔓 This project is licensed under the MIT License – feel free to use and modify it!
