# Case 1: Biased Hiring Tool – Amazon’s AI Recruiting Tool

## Overview

This project investigates the case of Amazon’s AI recruiting tool, which was found to be biased against female candidates. The included Jupyter notebook demonstrates how bias can arise in machine learning models due to historical data, shows the impact of bias on hiring outcomes, and implements practical steps to mitigate and audit for fairness.

---

## Contents

- **Case 1 Biased Hiring Tool.ipynb**  
  The main Jupyter notebook containing:
  - Background and source of bias in Amazon’s tool
  - Demonstration of bias in a simulated dataset
  - Data debiasing and model retraining
  - Fairness auditing using multiple metrics and calibration plots
  - Summary of proposed fixes

---

## Key Concepts

- **Source of Bias:**  
  The model learned gender bias from historical hiring data, penalizing resumes with female-associated terms.

- **Bias Demonstration:**  
  Analysis of the original dataset shows a disparate impact ratio of 0.0, with all male candidates hired and none of the female candidates hired.

- **Fixes Implemented:**
  1. **Debias Training Data:**  
     Remove gender-indicative terms and balance hiring outcomes.
  2. **Fairness Constraints in Model Design:**  
     Retrain the model and ensure gender is not a significant predictor.
  3. **Continuous Bias Auditing:**  
     Regularly check hiring rates and disparate impact ratios.

- **Fairness Metrics Used:**
  - Demographic Parity (Selection Rate)
  - Disparate Impact Ratio
  - Equal Opportunity (True Positive Rate Parity)
  - Equalized Odds (TPR and FPR)
  - Average Odds Difference
  - Calibration by Group

---

## How to Run

1. Open `Case 1 Biased Hiring Tool.ipynb` in Jupyter Notebook or VS Code.
2. Run each cell in order to see:
   - The biased dataset and its analysis
   - The debiasing process and model retraining
   - Fairness metrics and calibration plots

---

## Dependencies

- Python 3.7+
- pandas
- numpy
- scikit-learn
- matplotlib

Install dependencies with:
```bash
pip install pandas numpy scikit-learn matplotlib
```

---

## Summary Table: Proposed Fixes

| Fix                                   | Description                                                                                  |
|----------------------------------------|----------------------------------------------------------------------------------------------|
| Debias Training Data                   | Balance and anonymize data to remove historical and gender-based bias.                       |
| Fairness Constraints in Model Design   | Use algorithms and loss functions that enforce fairness during training.                     |
| Continuous Bias Auditing & Oversight   | Regularly monitor, audit, and review model outputs for bias, with human intervention as needed.|

---

## References

- [Amazon scraps secret AI recruiting tool that showed bias against women – Reuters](https://www.reuters.com/article/us-amazon-com-jobs-automation-insight-idUSKCN1MK08G)
- [Fairness in Machine Learning – scikit-learn documentation](https://scikit-learn.org/stable/)

---

## License

This project is for educational purposes