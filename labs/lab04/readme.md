# Geospatial Segmentation with SAM: Deep Learning for Tree Canopy Detection

- **Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); 
- **Teaching Assistant:** Liz Peng, lp36@uw.edu
- **Points Available** = 10

This lab introduces students to a geospatial deep learning pipeline using the **Segment Anything Model (SAM)** developed by Meta AI. Students will learn to apply SAM to high-resolution satellite imagery, perform feature segmentation using bounding box prompts, and export both raster and vector results for geospatial analysis.

The project not only builds technical fluency with foundational AI tools in geography but also invites reflection on how spatial knowledge is encoded, guided, and interpreted by machine learning models.

You will:

- Select or define a **Region of Interest (ROI)** using [geojson.io](https://geojson.io)  
- Download high-resolution **aerial imagery tiles** as a georeferenced GeoTIFF  
- Apply **Segment Anything Model (SAM)** to segment vegetation features using bounding box prompts  
- Convert the resulting raster mask into **vector GeoJSON** outputs  
- Visualize and compare model results using interactive mapping tools  
- Reflect on the use of deep learning in spatial reasoning and map interpretation

> **Guiding question:** How does deep learning enable new forms of geographic knowledge, and what are the limits of “segmenting anything” in a spatial context?

Click this button to launch the full lab on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1EseH1JT-iZGVGCtAT69vWta0s4TQVyIQ)

### Coding Experiments

Try one or more of the following:

- Replace the bounding box prompts with a new ROI from [geojson.io](https://geojson.io)  
- Use SAM to detect a different land cover class (e.g., water, rooftops, roads)  
- Change the `min_size` parameter in `region_groups()` and observe how the output polygon features change  
- Overlay outputs with external GIS layers such as land use or zoning data

### Written Reflection (choose two, 300–500 words total)

1. What kinds of geographic features did SAM identify most successfully in your region? Where did it fail?
2. How does the use of bounding boxes influence the segmentation results? Who defines the prompt?
3. What new opportunities or risks do AI-based tools like SAM introduce for geographic research or public mapping?
4. What limits did you observe when trying to apply this method to other types of land cover or imagery?

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

Thanks for Lewis "Yixiao" Liu's early exploration and testing. 