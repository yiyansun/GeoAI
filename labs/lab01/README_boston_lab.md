
# 🏡 Predicting Boston Housing Prices Using Machine Learning

**Author:** Bo Zhao, [jakobzhao@gmail.com](mailto:jakobzhao@gmail.com); **Points Available** = 50

This lab introduces students to a full machine learning pipeline for predicting housing prices using the classic Boston Housing Dataset. Students will learn to apply and compare multiple regression models while reflecting on the social structures embedded in housing data.

The project not only develops technical fluency in model building and evaluation but also guides students to critically examine how data reflects urban inequality, environmental injustice, and exclusionary zoning practices.

You will:

* Load and explore the Boston Housing Dataset
* Train and evaluate four regression models: OLS, SVR, Random Forest, and XGBoost
* Compare their performance using RMSE, R², and cross-validation
* Visualize feature importance and residuals
* Reflect on the ethical use of variables like CRIM, NOX, and PTRATIO

> **Guiding question:** How can machine learning reveal (or reinforce) spatial inequality in housing markets?

Click this button to launch the full lab on Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME/blob/main/predicting_boston_housing_prices.ipynb)

---

### 🔑 Key Files:

* `predicting_boston_housing_prices.ipynb`: The full lab notebook containing preprocessing, modeling, evaluation, and critical reflection.
* `boston_data.csv`: The cleaned Boston Housing Dataset (14 features + target).
* `Lab_Reflection_and_Extensions.md`: Optional extension experiments and critical reflection prompts.

---

### 📌 Final Reflection Prompts:

At the end of your lab, please answer **at least two** of the following questions (300–500 words total):

1. What does your best-performing model seem to “learn” about inequality?
2. Which variables might be ethically problematic to include (e.g., CRIM)? Why or why not?
3. How well does your model generalize across price ranges or neighborhoods?
4. What would an “equitable” housing model look like? What would it measure?

---

### 🧪 Optional Coding Experiments (Submit One)

Try one of the following in your notebook:

* Change Random Forest or XGBoost hyperparameters. How does performance shift?
* Remove a sensitive variable like CRIM or B. How does the model respond?
* Segment model error by price bracket (low, medium, high). What patterns emerge?

Submit results (plots or text) from your experiment as part of your Lab deliverable.

---

**Deliverables:**  
Submit your `.ipynb`, model outputs, and written reflection via Canvas.

**Note:** Please complete the assignment by the due date. Late work may receive a deduction unless prior arrangements are made.
