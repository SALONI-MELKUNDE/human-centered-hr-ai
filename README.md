# Explainable AI for Employee Attrition Prediction  
**Making HR Analytics Transparent with SHAP and LIME**

---

## 📑 Index
1. [Project Overview](#-project-overview)
2. [Objectives](#-objectives)
3. [Research Questions](#-research-questions)
4. [Why Explainable AI (XAI) for HR?](#-why-explainable-ai-xai-for-hr)
5. [Methodology & System Architecture](#-methodology--system-architecture)
6. [Machine Learning Models](#-machine-learning-models)
7. [Explainability Methods](#-explainability-methods)
   - [SHAP](#shap-shapley-additive-explanations)
   - [LIME](#lime-local-interpretable-model-agnostic-explanations)
8. [SHAP vs LIME Comparison](#-shap-vs-lime-comparison)
9. [Employee Segmentation & Survival Analysis](#-employee-segmentation--survival-analysis)
10. [HR Decision Support & Actions](#-hr-decision-support--actions)
11. [Research Contributions](#-research-contributions)
12. [Contact & Feedback](#-thank-you-for-exploring-the-jobsatisfaction_mlproject-)

---

## 📌 Project Overview
Employee attrition prediction is a critical problem in Human Resource (HR) analytics. While machine learning (ML) models can predict employee turnover with high accuracy, most models act as *black boxes*, limiting trust and practical adoption in HR decision-making.

This project develops an **end-to-end Explainable AI (XAI) pipeline** that combines predictive modeling with **SHAP** and **LIME** explanations to make attrition predictions transparent, interpretable, and actionable for HR professionals.

The study further extends traditional attrition prediction by incorporating **employee clustering** and **survival analysis** to identify high-risk groups and early-leaving employee segments.

---

## 🎯 Objectives
- Predict employee attrition using machine learning models
- Identify key drivers of attrition
- Apply **SHAP** and **LIME** to explain model predictions
- Compare explanation quality, stability, and clarity
- Translate model explanations into **practical HR retention actions**
- Identify high-risk employee groups using clustering
- Quantify early attrition risk using survival analysis

---

## ❓ Research Questions
- **RQ1:** How effectively can machine learning models predict employee attrition?
- **RQ2:** How do SHAP and LIME explain employee attrition predictions individually?
- **RQ3:** Which explainability method is clearer and more stable?
- **RQ4:** How can explainable model insights improve HR decision-making?

---

## 🧠 Why Explainable AI (XAI) for HR?
- Makes AI decisions transparent and trustworthy
- Explains *why* employees leave (e.g., **OverTime**, **JobSatisfaction**)
- Enables targeted and personalized retention strategies
- Supports responsible, fair, and bias-aware HR analytics
- Improves stakeholder confidence in AI-driven decisions

---

## 🏗 Methodology & System Architecture
The project follows a **human-centered ML pipeline**:

1. Data preprocessing and feature engineering  
2. Handling class imbalance using **SMOTE**
3. Model training and evaluation
4. Global and local explainability using SHAP and LIME
5. Employee segmentation using clustering
6. Survival analysis to estimate early-leaving risk
7. Translation of insights into HR actions

---

## 🤖 Machine Learning Models
Three models were trained and evaluated using cross-validation:

- **Logistic Regression**
- **Random Forest**
- **XGBoost**

### Best Performing Model
- **Logistic Regression**
- Cross-validated ROC-AUC: **0.830 ± 0.026**
- Test ROC-AUC: **0.80**
- Confusion matrix shows reasonable recall for leavers

---

## 🔍 Explainability Methods

### SHAP (SHapley Additive exPlanations)
- Provides **global and local explanations**
- Produces consistent feature rankings
- High stability across runs  
- Key drivers consistently identified:
  - OverTime
  - StockOptionLevel
  - JobSatisfaction
  - WorkLifeBalance

### LIME (Local Interpretable Model-agnostic Explanations)
- Explains individual predictions
- Useful for personalized HR decisions
- Shows higher variability across runs
- Moderate local fidelity

---

## 📊 SHAP vs LIME Comparison
| Aspect | SHAP | LIME |
|------|------|------|
| Explanation scope | Global & Local | Local |
| Stability | High | Moderate |
| Feature ranking consistency | High (Spearman = 0.717) | Variable |
| Interpretability for policy | Strong | Limited |
| Interpretability for individuals | Good | Strong |

**Conclusion:** SHAP provides clearer and more stable explanations, while LIME is useful for individualized case analysis.

---

## 👥 Employee Segmentation & Survival Analysis
To extend prediction insights:
- Employees were clustered into distinct risk groups
- Survival analysis quantified **time-to-attrition**

### Key Findings
- Employees with **OverTime** leave fastest (Hazard Ratio = **3.06**)
- Frequent job changers exit earlier (HR = **1.13**)
- Higher job and environment satisfaction reduce early attrition (HR < 1)
- Better work–life balance slows attrition
- Longer tenure with current manager improves retention (HR = **0.71**)

---

## 🧩 HR Decision Support & Actions
Model explanations were translated into actionable HR strategies:
- Overtime monitoring and workload rebalancing
- Targeted retention programs for high-risk clusters
- Personalized interventions using LIME explanations
- Policy-level changes informed by SHAP global drivers
- Support for ethical, transparent, and responsible AI adoption in HR

---

## 🏆 Research Contributions
- Developed a **balanced ML pipeline** using SMOTE
- Compared three ML models for attrition prediction
- Delivered a systematic comparison of **SHAP vs LIME**
- Identified stable global attrition drivers
- Linked XAI insights to **practical HR retention strategies**
- Introduced clustering and survival analysis for deeper risk understanding
- Promoted **human-centered and transparent AI** for HR analytics

---

## Thank you for exploring the human-centered-hr-ai! 🎉

- **If you have any questions or suggestions, feel free to open an issue or reach out.** 💬 📬
