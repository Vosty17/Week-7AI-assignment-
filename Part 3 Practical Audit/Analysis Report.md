# Analysis Report

**Fairness Analysis of COMPAS Risk Scores Using AI Fairness 360**

This project analyzed racial bias in the COMPAS recidivism risk scores using IBM’s AI Fairness 360 toolkit. The COMPAS dataset, which includes demographic and criminal history features, was explored and preprocessed to enable fairness assessment. The analysis focused on the two-year recidivism prediction, with race as the protected attribute.

**Key Findings:**

> **Major Findings:**
> 
> - **Disparities in Recidivism Rates:** Initial analysis revealed clear differences in recidivism rates across racial groups.
> - **Bias in Risk Scores:** Disparate impact and statistical parity difference metrics indicated bias against unprivileged groups (e.g., African-American defendants).
> - **Model Fairness Gaps:** The logistic regression model showed significant differences in false positive rates, false negative rates, and equal opportunity between racial groups.
> - **Visualization Evidence:** Confusion matrices and ROC curves by race confirmed that the model was less accurate and more likely to misclassify unprivileged group members.

**Remediation Steps:**

To address these biases, we applied the Reweighing algorithm from AIF360, which adjusts instance weights to reduce the influence of bias in the training data. Post-mitigation fairness metrics showed improvement in disparate impact and statistical parity difference, indicating a reduction in bias. However, some disparities persisted, suggesting that further remediation may be necessary.

**Recommendations:**

- Use bias mitigation algorithms such as reweighing or adversarial debiasing during model training.
- Regularly monitor fairness metrics (e.g., disparate impact, equal opportunity difference) alongside accuracy.
- Consider additional features or alternative modeling approaches to further reduce bias.
- Engage stakeholders to interpret results and ensure that remediation aligns with ethical and legal standards.

In summary, while mitigation techniques can reduce bias, ongoing evaluation and a multi-faceted approach are essential for fair and responsible use of risk assessment tools like COMPAS.
