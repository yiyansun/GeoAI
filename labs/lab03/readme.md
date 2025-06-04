# 🧪 Lab 3: Using YOLO to Detect Informal Structures in Urban Spaces

## 🎯 Objective

This lab explores how a pre-trained object detection model (YOLOv8) performs in recognizing both **standard** and **informal/irregular** urban structures. The goal is not only to understand the technical workflow of object detection but also to engage critically with the socio-spatial biases embedded in AI systems.

Students will:

- Apply YOLOv8 to images of both structured and unstructured urban environments.
- Evaluate detection performance differences, especially in recognizing objects like **homeless tents**, **makeshift shelters**, and **small or semi-legal constructions**.
- Reflect on the political and epistemological implications of what the AI "sees" and "misses".

---

## 🧰 Workflow

> This lab follows a **fixed pipeline**. Students are not expected to define their own categories or custom training sets for now.

### Step 1: Dataset Preparation

You will be provided with two sets of urban imagery:

1. **Structured Urban Scenes**: commercial districts, residential zones, clean sidewalks, etc. These are environments where YOLOv8 performs well.
2. **Informal/Marginal Spaces**: underpasses, alleyways, tent encampments, and informal housing. These are challenging for standard models.

> Images will be collected from sources such as Google Street View, Mapillary, or instructor-provided datasets.

---

### Step 2: Run YOLOv8 Object Detection

Using a pre-trained YOLOv8 model:

- Run detection on both datasets.
- Export detection outputs: bounding boxes, object classes, and confidence scores.
- Note which types of objects are reliably detected — and which are consistently missed.

---

### Step 3: Visualize & Compare Results

- Overlay YOLO detection boxes on the original images.
- Compare metrics between the two datasets:
  - Average number of objects detected per image
  - Class distribution of detected objects
  - Mean confidence scores
  - Detection gaps (areas with visible but undetected structures)

---

## 🧠 Critical Reflection

Students are required to include a short reflection (~300 words) in their lab report, addressing questions like:

- **Algorithmic Blind Spots**: What does it mean when the model fails to detect informal structures like tents or shacks?
- **Spatial Bias in Training Data**: YOLO is trained on COCO/ImageNet datasets. Are these biased toward orderly, middle-class environments?
- **Gentrification & Visibility**: In areas undergoing gentrification, do detection failures reflect broader processes of displacement and erasure?
- **Implications for Urban AI**: How could such limitations impact real-world applications like urban planning or automated surveillance?

---

## 📦 Optional Extension (Instructor-led)

If time and resources permit, the following activities may be explored:

- Use Meta’s Segment Anything Model (SAM) to visualize what YOLO might have missed.
- Manually annotate 10–20 informal structures, retrain YOLO on this micro-dataset, and compare performance.
- Import undetected areas into GIS as polygons, analyze spatial correlation with zoning maps, eviction data, or income layers.

---

## ✅ Deliverables

- Processed images with YOLO detection results (structured vs informal)
- A short report (markdown or PDF) including:
  - A summary of findings
  - Visualizations
  - Critical reflection section

---

## 🛠️ Tools

- Python (YOLOv8 via `ultralytics`)
- Google Colab (provided starter notebook)
- Sample datasets
- Optional: Segment Anything, QGIS, or geopandas for spatial overlays

---

## 💬 Closing Thought

> *"What the algorithm sees — and does not see — shapes how we govern space."*

This lab invites you to go beyond model performance, toward a deeper understanding of how AI encodes, amplifies, or ignores the complexities of urban life.
