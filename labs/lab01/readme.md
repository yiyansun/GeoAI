# Predicting Boston Housing Prices Using Machine Learning

**Author:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); **Points Available** = 50

This lab introduces students to a full machine learning pipeline for predicting housing prices using the classic Boston Housing Dataset. Students will learn to apply and compare multiple regression models while reflecting on the social structures embedded in housing data.

The project not only develops technical fluency in model building and evaluation but also guides students to critically examine how data reflects urban inequality, environmental injustice, and exclusionary zoning practices.

You will:

* Load and explore the Boston Housing Dataset
* Train and evaluate four regression models: OLS, SVR, Random Forest, and XGBoost
* Compare their performance using RMSE, R², and cross-validation
* Visualize feature importance and residuals
* Reflect on the ethical use of variables like CRIM, NOX, and PTRATIO

> **Guiding question:** How can machine learning reveal (or reinforce) spatial inequality in housing markets?

Click this button to launch the full lab on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jakobzhao/geog428/blob/main/labs/lab01/predicting_boston_housing_prices.ipynb)

---
### 🧪 Coding Experiments：

Try one of the following in your notebook:

* Change Random Forest or XGBoost hyperparameters. How does performance shift?
* Remove a sensitive variable like CRIM or B. How does the model respond?
* Segment model error by price bracket (low, medium, high). What patterns emerge?

---

### 📌 Written Reflection:

At the end of your lab, please answer **at least two** of the following questions (300–500 words total):

1. What does your best-performing model seem to “learn” about inequality?
2. Which variables might be ethically problematic to include (e.g., CRIM)? Why or why not?
3. How well does your model generalize across price ranges or neighborhoods?
4. What would an “equitable” housing model look like? What would it measure?

---

## ✅ Deliverables

Your submission must include **two parts**:

1. **Coding Experiments:** Add your experiment(s) to the notebook and generate any plots, outputs, or analysis.
2. **Written Reflection:** Submit your answers to the reflection prompts above.

Please export both parts into a **Word document or PDF** and upload to **Canvas**.

**Note:** Lab assignments are required to be submitted electronically to Canvas unless stated otherwise. Efforts will be made to have them graded and returned within one week after they are submitted.Lab assignments are expected to be completed by the due date. ***A late penalty of at least 10 percentage units will be taken off each day after the due date.*** If you have a genuine reason(known medical condition, a pile-up of due assignments on other courses, ROTC,athletics teams, job interview, religious obligations etc.) for being unable to complete work on time, then some flexibility is possible. However, if in my judgment you could reasonably have let me know beforehand that there would likely be a delay, and then a late penalty will still be imposed if I don't hear from you until after the deadline has passed. For unforeseeable problems,I can be more flexible. If there are ongoing medical, personal, or other issues that are likely to affect your work all semester, then please arrange to see me to discuss the situation. There will be NO make-up exams except for circumstances like those above.