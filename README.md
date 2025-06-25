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

# 2. Create & activate a virtual environment
python -m venv .venv

# 3. Install Python dependencies
pip install -r requirements.txt

# 4. Launch the notebook
jupyter notebook code_supervised_learning_coursework_1.ipynb
```

# Compiling the report

```bash
latexmk -pdf main.tex            
```

```

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
| Q10      | 3 / 10  | Your condition holds for small β, which is incorrect; the correct condition holds only for large β. |
| Q11a     | 1 / 1   |                                                                                                     |
| Q11b     | 1 / 1   |                                                                                                     |
| Q11c     | 2 / 2   |                                                                                                     |
| Q11d     | 2 / 2   |                                                                                                     |
| Q11e     | 2 / 2   |                                                                                                     |
| Q11f     | 2 / 2   |                                                                                                     |
| Q11gi    | 1 / 2   |                                                                                                     |
| Q11gii   | 2 / 2   |                                                                                                     |
| Q11giii  | 2 / 2   |                                                                                                     |


