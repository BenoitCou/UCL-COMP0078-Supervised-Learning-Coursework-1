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

# 2. Create & activate a virtual environment  (optional but recommended)
python -m venv .venv
source .venv/bin/activate           # Windows: .venv\Scripts\activate

# Install Python dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook code_supervised_learning_coursework_1.ipynb
# or (modern UI):
jupyter lab


##Compiling the report
A full LaTeX distribution is required (TeX Live 2023+, MiKTeX, or Mac TeX).

latexmk -pdf main.tex            
The generated main.pdf is ready for submission.
