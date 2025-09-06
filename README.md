# Statistical-Simulation-Higher-Dimensional-Data-Analysis


**Course Project | Data Science Lab II (MTH209)**  
*Jan 2025 – Apr 2025 | Mentor: Prof. Subhra Shankar Dhar, Dept. of Mathematics & Statistics, IIT Kanpur*  

This repository contains simulation-based assignments and projects completed as part of the MTH209: Data Science Lab II course. The focus was on applying **Monte Carlo methods, statistical tests, regression techniques, and parallel computing** for large-scale data analysis.  

---

## Key Topics & Contributions  

### 1. Monte Carlo Simulation of *e* and *π*  
- Estimated **Euler’s number (e)** using:
  - (n+1)-sided dice rolls  
  - Factorial-based random permutations  
  - Geometric probability & integration methods  
  - Monte Carlo summation (uniform randoms)  
- Estimated **π** via **high-dimensional sphere volume approximation**.  
- Validated randomness with the **Runs Test**.  

### 2. Normality & Distributional Analysis  
- Normalized large **sunspot dataset** and tested normality with:  
  - **Shapiro–Wilk, Kolmogorov–Smirnov, and Cramér–von Mises tests**.  
- Complementary visual checks: **Q–Q plots, boxplots, histograms**.  
- Findings: dataset deviates from perfect normality (skewness, heavy tails).  

### 3. Regression & Robustness  
- Compared **Least Absolute Deviations (LAD)** vs. **Least Squares Estimator (LSE)**.  
- Evaluated robustness under outliers using error metrics and fitted regression curves.  

### 4. Contour Plots & Mode Detection  
- Generated **contour density plots** for:  
  - Simulated unimodal and bimodal distributions.  
  - Real-world datasets (students’ performance, stellar properties).  
  - Image-based color distributions (HSV space).  
- Used **Kernel Density Estimation (KDE)** for unimodal vs. bimodal detection.  

### 5. Copula-Based Integration  
- Applied **copula theory** to compute multivariate integrals.  
- Monte Carlo convergence analysis with varying dimensions (n) and sample sizes (N).  

### 6. Parallel Computing & High-Dimensional Simulation  
- Designed a **parallel simulation framework in R** using `foreach` + `doParallel`.  
- Generated **10¹¹+ standard normal variates** with chunking (10⁷ per core).  
- Achieved:  
  - Scalable performance (speedup ≈ 6.5× on 8 cores).  
  - Memory efficiency (streaming sums & variances only).  
  - Verified global mean ≈ 0, variance ≈ 1.  

---

## 🛠 Tech Stack  
- **Language:** R  
- **Libraries:** `ggplot2`, `foreach`, `doParallel`, `MASS`, `zoo`, `imager`, `gridExtra`, `goftest`  
- **Methods:** Monte Carlo Simulation, Kernel Density Estimation (KDE), Copula Theory, Statistical Tests, Parallel Computing  

---

## Sample Outputs  
- Convergence plots for estimating *e* and *π*.  
- Normality test results (W-statistic, KS D-value, CvM ω²).  
- Contour plots (unimodal, bimodal, real datasets, image-based).  
- Parallel runtime scaling vs. chunk size.  

---

## 🚀 How to Run  
1. Clone the repo:  
   ```bash
   git clone https://github.com/your-username/statistical-simulation.git
   cd statistical-simulation
