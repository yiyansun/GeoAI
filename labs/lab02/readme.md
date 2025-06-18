# Downscaling Urban Heat of Seattle Using Random Forests

- **Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); 
- **Teaching Assistant:** Liz Peng, lp36@uw.edu
- **Points Available** = 10

This lab introduces students to a progressive modeling workflow for **downscaling coarse-resolution land surface temperature (LST)** to finer spatial scales in the Seattle metropolitan area using satellite data and machine learning.  
By using **Google Earth Engine**, **Sentinel-2 imagery**, and **Landsat 8 LST products**, students will explore how vegetation, built-up surfaces, and geographic context influence urban heat patterns.

The lab emphasizes both **technical modeling fluency** and **critical spatial reasoning**, guiding students through model comparison, spatial pattern analysis, and the epistemological questions behind predictive GeoAI.

You will:

- Authenticate and access Google Earth Engine using your own GCP project
- Compute vegetation and built-up indices such as **NDVI**, **NDBI**, and **NDWI**
- Build and evaluate multiple models
- Compare model performance using **R²**, **RMSE**, **MAE**, and scatter plots
- Visualize and interpret downscaled temperature maps
- Reflect on the assumptions and implications of spatial downscaling

> **Guiding Question:** How does the choice of input features—spectral, index-based, or geographic—change our ability to model and interpret urban heat?

Click this button to launch the full lab on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Y7wHJ9UGL9OiVIypfvudU1M_duXSnZCz)

### Coding Experiments:

Choose **at least one** of the following and add your experiment(s) to the notebook:

- Try a different index (e.g., EVI or SAVI) and substitute it into the model. Does performance improve?
- Use fewer features (e.g., only visible bands). What happens to accuracy?
- Try tuning the number of trees in the Random Forest (e.g., `n_estimators=100` vs `500`). How sensitive is the result?
- Evaluate model bias by region: Which ROI has the highest prediction error?

### ✍Written Reflection:

At the end of your lab, answer **at least two** of the following questions (300–500 words total):

1. Which model performed best in your results, and why do you think that is?
2. What kinds of features (spectral vs. geographic) contributed most to model accuracy?
3. Does including latitude/longitude raise any conceptual or practical concerns?
4. What are the risks of using machine learning to represent geographic phenomena?
5. What does this exercise teach us about how AI “sees” the city?

---

## ✅ Deliverables

All deliverables must be submitted via **Canvas Discussion Board**, under the thread corresponding to this lab. Your Canvas post for this lab should look like:

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