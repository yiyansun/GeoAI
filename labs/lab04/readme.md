# Geospatial Segmentation with SAM: Deep Learning for Tree Canopy Detection

> Bo Zhao | zhaobo@uw.edu | Department of Geographhy, University of Washington - Seattle

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


## ✅ Deliverables

Your submission must include **two parts**:

1. **Notebook:** Include your code and at least one segmentation result, with proper map visualizations and layer explanations.
2. **Reflection:** Add your written responses to the reflection prompts at the end of the notebook (or submit separately).

Please export both parts into a **PDF** or **Word document** and upload to **Canvas**.

> **Note:** Lab assignments must be submitted electronically to Canvas by the due date. Late submissions will incur a 10% penalty per day unless prior notice is given for valid reasons such as illness, academic conflicts, or personal emergencies. Flexibility is possible with timely communication, but make-up exams or extensions will only be granted in documented, exceptional cases.
