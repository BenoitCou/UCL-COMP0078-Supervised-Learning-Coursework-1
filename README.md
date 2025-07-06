# COMP0078 — Supervised Learning • Coursework 1  
MSc in Machine Learning, University College London (2024 / 25)

This repository contains all the material submitted for **Coursework 1** of the COMP0078 *Supervised Learning* module.  
It includes:

| Path | Description |
|------|-------------|
| `main.tex`          | LaTeX source of the written report (compiled PDF shows all answers, figures and tables). |
| `images/`           | Auxiliary figures referenced by `main.tex`. |
| `code_supervised_learning_coursework_1.ipynb` | Jupyter notebook implementing every experiment required in the coursework (polynomial fits, bias/variance exploration, Kernel Ridge Regression, k-NN, etc.). |
| `boston_filtered.csv` | Pre-filtered Boston Housing dataset used in Part 1 & 3. |
| `Coursework1_Task.pdf` | The questions of the coursework  |


---

## Quick-start

```bash
# 1. Clone the repo
git clone https://github.com/BenoitCou/UCL-COMP0078-Supervised-Learning-Coursework-1
cd UCL-COMP0078-Supervised-Learning-Coursework-1

# 2. Install Python dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook code_supervised_learning_coursework_1.ipynb
```

# Compiling the report

```bash
latexmk -pdf main.tex            
```
# Coursework Overview

**Part I – Supervised‑learning experiments (50 % of mark)**

- **Polynomial regression on toy data** — fits of degree 1–18, visualised together with training points; explicit equations for low‑order models.

- **Bias/variance & over‑fitting analysis** — training vs test MSE curves, log‑scaled, averaged over 100 Monte‑Carlo repeats.

- **Boston Housing study**

  - *Baseline*: constant predictor.

  - *Single‑attribute & full linear regression*: ordinary least squares with bias term.

  - *Gaussian Kernel Ridge Regression*: 5‑fold CV over 2−40…−26 for γ and 27…13 for σ, repeated on 20 random splits.

  - **Result table** summarising mean ± s.d. MSE for all methods.

**Part II – k‑Nearest Neighbours (20 %)**

- Pure‑Python k‑NN implementation.

- **Voted‑centre hypothesis visualisation** on the unit square with v = 3, mirroring the coursework’s Figure 1.

- **Protocol A**: generalisation error vs k∈[1, 49] using 4 000 train / 1 000 test points, averaged over 100 random draws.

- **Protocol B**: optimal k as a function of training‑set size m∈{100,…,4 000}, averaged over 100 runs.

- Commentary on the bias–variance trade‑off observed in both experiments.

**Part III – Theory & Proofs (30 %)**

- **Positive‑definite kernel modification** — conditions on c for $$K_c(x,z) = c + \sum x_i z_i$$  .

- **Gaussian kernel vs 1‑NN** — shows how choosing β→∞ lets kernel ridge regression emulate 1‑NN.

- **No‑Free‑Lunch theorem** — step‑by‑step proof (questions 11a–f) and discussion of learnability implications (11g).


## Marks Obtained

*Grade*: 95 / 100

| Question | Score   | Comments                                                                                            |
| -------- | ------- | --------------------------------------------------------------------------------------------------- |
| Q1       | 5 / 5   |                                                                                                     |
| Q2       | 10 / 10 |                                                                                                     |
| Q3       | 5 / 5   |                                                                                                     |
| Q4       | 10 / 10 |                                                                                                     |
| Q5       | 20 / 20 |                                                                                                     |
| Q6       | 5 / 5   |                                                                                                     |
| Q7       | 7 / 7   |                                                                                                     |
| Q8       | 6 / 8   | Incorrect explanation; should explicitly describe how point density in an ε-neighbourhood changes.  |
| Q9a      | 2 / 3   | Condition must hold for all x and z, hence c ≥ 0.                                                   |
| Q9b      | 0 / 2   | c acts as a bias but not a regulariser; c > 0 does not impact the solution.                         |
| Q10      | 10 / 10 |                                                                                                     |
| Q11a     | 1 / 1   |                                                                                                     |
| Q11b     | 1 / 1   |                                                                                                     |
| Q11c     | 2 / 2   |                                                                                                     |
| Q11d     | 2 / 2   |                                                                                                     |
| Q11e     | 2 / 2   |                                                                                                     |
| Q11f     | 2 / 2   |                                                                                                     |
| Q11gi    | 1 / 2   |                                                                                                     |
| Q11gii   | 2 / 2   |                                                                                                     |
| Q11giii  | 2 / 2   |                                                                                                     |


