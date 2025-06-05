# Downscaling Land Surface Temperature in Seattle: Exploring Urban Heat and Modeling Strategies

**Author:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); **Points Available** = 50

This lab introduces students to a progressive modeling workflow for **downscaling coarse-resolution land surface temperature (LST)** to finer spatial scales in the Seattle metropolitan area using satellite data and machine learning.  
By using **Google Earth Engine**, **Sentinel-2 imagery**, and **Landsat 8 LST products**, students will explore how vegetation, built-up surfaces, and geographic context influence urban heat patterns.

The lab emphasizes both **technical modeling fluency** and **critical spatial reasoning**, guiding students through model comparison, spatial pattern analysis, and the epistemological questions behind predictive geospatial AI.

You will:

- Authenticate and access Google Earth Engine using your own GCP project
- Compute vegetation and built-up indices such as **NDVI**, **NDBI**, and **NDWI**
- Build and evaluate multiple models:
  - Linear regression with NDVI
  - Random Forest with NDVI
  - Random Forest with multi-band + index features
  - Random Forest with additional **geographic context**
- Compare model performance using **R²**, **RMSE**, **MAE**, and scatter plots
- Visualize and interpret downscaled temperature maps
- Reflect on the assumptions and implications of spatial downscaling

> **Guiding Question:** How does the choice of input features—spectral, index-based, or geographic—change our ability to model and interpret urban heat?

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jakobzhao/geog428/blob/main/labs/lab02/seattle_lst_downscaling_with_rf.ipynb)

---

### 🔬 Coding Experiments:

Choose **at least one** of the following and add your experiment(s) to the notebook:

- Try a different index (e.g., EVI or SAVI) and substitute it into the model. Does performance improve?
- Use fewer features (e.g., only visible bands). What happens to accuracy?
- Try tuning the number of trees in the Random Forest (e.g., `n_estimators=100` vs `500`). How sensitive is the result?
- Evaluate model bias by region: Which ROI has the highest prediction error?

---

### ✍️ Written Reflection:

At the end of your lab, answer **at least two** of the following questions (300–500 words total):

1. Which model performed best in your results, and why do you think that is?
2. What kinds of features (spectral vs. geographic) contributed most to model accuracy?
3. Does including latitude/longitude raise any conceptual or practical concerns?
4. What are the risks of using machine learning to represent geospatial phenomena?
5. What does this exercise teach us about how AI “sees” the city?

---

## ✅ Deliverables

Your submission must include **two parts**:

1. **Coding Experiments:** Add code and outputs to the notebook. Include comments describing your experiment.
2. **Written Reflection:** Submit your answers to the reflection prompts as either a new cell in the notebook or as a separate PDF/Word file.

Please export both parts into a **PDF or Word document** and upload to **Canvas** by the due date.

**Note:** Late submissions will receive a 10% penalty per day unless approved in advance. If you encounter technical or personal issues, please reach out early. Flexibility is possible with communication.
