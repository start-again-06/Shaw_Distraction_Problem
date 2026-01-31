# Shaw Distraction Problem  
## Singular Value Decomposition (SVD) Analysis

---

## System Overview
This project analyzes the **Shaw distraction inverse problem** using **Singular Value Decomposition (SVD)** to study numerical instability and regularization in ill-conditioned systems. The implementation demonstrates how filtering and regularization techniques improve solution stability when solving inverse problems.

The workflow combines matrix construction, SVD-based decomposition, regularization parameter tuning, and visual diagnostics.

---

## High-Level Architecture

### Data and Discretization Layer
- Discretized domain based on the Shaw problem formulation  
- Transformation matrix constructed using trigonometric functions  
- Numerical safeguards applied to handle singular behavior  

---

### Matrix Construction Layer
- Weight matrix **G** generated from analytical expressions  
- Represents the forward operator of the inverse problem  
- Ill-conditioned by design to illustrate numerical instability  

---

### Decomposition Layer
**Method:** Singular Value Decomposition  

$$
\[
G = U \cdot S \cdot V^T
\]
$$

- Decomposes system into orthogonal basis components  
- Extracts singular values to analyze conditioning  
- Evaluates rank and numerical sensitivity  

---

### Regularization Layer
**Approach:** Tikhonov-style spectral filtering  

- Iterative evaluation across a range of regularization parameters \($$\alpha \$$)  
- Filter function applied to singular values:

$$
\[
f(i) = \frac{s(i)^2}{s(i)^2 + \alpha^2}
\]
$$

- Suppresses contributions from small singular values  
- Balances stability and reconstruction accuracy  

---

### Solution Reconstruction Layer
- Computes regularized inverse solutions  
- Evaluates solution norm and reconstruction error  
- Tracks trade-off behavior across regularization parameters  

---

### Visualization & Diagnostics Layer
- Stair-step plots for filtered spectral components  
- Log-log plots of reconstruction error versus solution norm  
- Visual identification of optimal regularization parameter  

---

## Execution Flow
1. Discretize the Shaw problem domain  
2. Construct transformation matrix G  
3. Perform Singular Value Decomposition  
4. Analyze singular values and conditioning  
5. Apply spectral filtering across multiple α values  
6. Reconstruct regularized solutions  
7. Visualize error-norm trade-offs using log-log plots  

---

## Results & Insights
- Small singular values dominate numerical instability  
- SVD reveals sensitivity structure of the inverse problem  
- Regularization suppresses unstable components  
- Log-log analysis helps identify optimal regularization strength  

---

## Scalability & Extensibility
- Can be extended to other ill-posed inverse problems  
- Alternative regularization methods can be incorporated  
- Useful for testing parameter selection strategies  
- Suitable for numerical analysis and inverse problem research  

---

## Applications
- Inverse problem regularization studies  
- Numerical linear algebra education  
- Ill-conditioned system analysis  
- Validation of SVD-based filtering techniques  

---

## Dependencies
- MATLAB or GNU Octave  

---

## License
MIT License. Free to use, modify, and distribute for academic and research purposes.
