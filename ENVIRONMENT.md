# Environment Setup

This document describes the Python environment required to run the  
**Explainable AI for Employee Attrition Prediction** project.

The environment specification is derived directly from the libraries and tools
used in the Jupyter Notebook.

---

## 📥 Cloning the Repository

To obtain a local copy of the project, clone the repository using Git:

```bash
git clone https://github.com/SALONI-MELKUNDE/human-centered-hr-ai.git
```

Navigate into the project directory:

```bash
cd human-centered-hr-ai
```

---

Ensure Git is installed on your system before running the above commands.

---

## 🐍 Python Version

The project was developed and tested using:

- Python 3.9 or higher (Recommended: Python 3.9 or Python 3.10)

---

## 📦 Required Python Libraries

Core Data & Numerical Computing

- numpy
- pandas
- scipy

Data Visualization

- matplotlib
- seaborn
- plotly

Machine Learning

- scikit-learn
- xgboost
- imbalanced-learn

Explainable AI (XAI)

- shap
- lime

Survival Analysis

- lifelines

---

## ⚙️ Local Environment Setup

1️⃣ Create a virtual environment

```bash
python -m venv venv
```

2️⃣ Activate the virtual environment

```bash
# Windows
venv\Scripts\activate
```

```bash
# macOS / Linux
source venv/bin/activate
```

3️⃣ Install required libraries

```bash
pip install numpy pandas scipy matplotlib seaborn plotly scikit-learn xgboost imbalanced-learn shap lime lifelines
```

---


## 🌐 Deployment Notes

- The project outputs are designed to be used as static artifacts.
- No server-side Python execution is required.
- All computations are performed locally before generating final outputs.

---

## 📌 Reproducibility Guidelines

To ensure consistent and reproducible results:

- Use the same Python version.
- Install the listed libraries in a clean environment.
- Set random seeds where applicable.
- Run the notebook sequentially from start to finish.

---

## 📬 Support & Troubleshooting

If environment-related issues occur:

- Confirm Python is correctly installed and accessible.
- Verify successful installation of all listed libraries.
- Some libraries (such as xgboost and shap) may require additional system dependencies depending on the operating system.
