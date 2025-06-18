# Predicting Boston Housing Prices Using Machine Learning

- **Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); 
- **Teaching Assistant:** Liz Peng, lp36@uw.edu
- **Points Available** = 10

This lab introduces students to a full machine learning pipeline for predicting housing prices using the classic Boston Housing Dataset. Students will learn to apply and compare multiple regression models while reflecting on the social structures embedded in housing data.

The project not only develops technical fluency in model building and evaluation but also guides students to critically examine how data reflects urban inequality, environmental injustice, and exclusionary zoning practices.

You will:

* Load and explore the Boston Housing Dataset
* Train and evaluate four regression models: OLS, SVR, Random Forest, and XGBoost
* Compare their performance using RMSE, R², and cross-validation
* Visualize feature importance and residuals
* Reflect on the ethical use of variables like CRIM, NOX, and PTRATIO

> **Guiding question:** How can machine learning reveal (or reinforce) spatial inequality in housing markets?

Click this button to launch the full lab on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1NlXCv1xvQd4aJD_ynHOQY7t3bMbJoK0S)

### Coding Experiments：

Try one of the following in your notebook:

* Change Random Forest or XGBoost hyperparameters. How does performance shift?
* Remove a variable like CRIM. How does the model respond?
* Segment model error by price bracket (low, medium, high). What patterns emerge?


### Written Reflection:

At the end of your lab, please answer **at least two** of the following questions (300–500 words total):

1. What does your best-performing model seem to “learn” about inequality?
2. Which variables might be ethically problematic to include (e.g., CRIM, PTRATIO)? Why or why not?
3. How well does your model generalize across price ranges or neighborhoods?
4. What would an “equitable” housing model look like? What would it measure?

---

## ✅ Deliverables

All deliverables must be submitted via **Canvas Discussion Board**, under the thread corresponding to this lab (e.g., “Lab  01”). Your Canvas post for this lab should look like:

```
My Colab Notebook: https://colab.research.google.com/drive/your_unique_link_here

Reflection:

1. [Your response to question 1 here...]
2. [Your response to question 2 here...]
```

You must complete your entire code in a single Google Colab notebook. Your Colab notebook must be **Sharable with both the Instructor (`zhaobo@uw.edu`) and the TA (`lp36@uw.edu`)**

> To share correctly:
> 1. Click the **“Share”** button in the top-right corner of your Colab window.
> 2. Under **“Add people and groups”**, enter:  
>    `zhaobo@uw.edu`, `lp36@uw.edu`
> 3. Set their access to "**Editor**".
> 4. Click **“Send”**.

⚠️ **Failure to share your notebook properly will result in an automatic deduction of at least 10% of your lab grade. We take this seriously because improper sharing causes delays for everyone. Please double-check your settings before submitting!**

At the **very top of your Colab**, include the following academic integrity statement:

```markdown
"I affirm that this notebook was completed independently and that I did not reference or use anyone else's code."
```

**Note:** Lab assignments must be submitted electronically to Canvas by the due date. Late submissions will incur a 10% penalty per day unless prior notice is given for valid reasons such as illness, academic conflicts, or personal emergencies. Flexibility is possible with timely communication, but make-up exams or extensions will only be granted in documented, exceptional cases.

#### Acknowledgement

This lab is largely built upon Haowei Wei's early contribution, and later Lewis "Yixiao" Liu helped me testing and editing the script.