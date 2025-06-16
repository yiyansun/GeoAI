# Identifying Homeless Camps Using YOLO

**Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu), **Points Available** = 50

This lab introduces students to the use of **deep learning for geospatial object detection** using the YOLOv8 model. You will start by exploring the results of a pretrained YOLO model and then proceed to **fine-tune a model** using your own annotated dataset to detect a novel class: **"camp"** — referring to **homeless camps** such as tents or makeshift shelters in urban environments.

The lab also critically engages with the ethical implications of applying automated detection systems to socially sensitive phenomena.

You will:

- Run a pretrained YOLOv8 model on urban imagery
- Annotate and prepare a training dataset using LabelImg
- Fine-tune YOLOv8 on the "camp" class
- Reflect on the **risks and benefits** of using deep learning to recognize **homeless camps**

> **Guiding question:** How can deep learning models like YOLO shape — and perhaps distort — our understanding of spatial visibility, homelessness, and social intervention?

---

Click this button to launch the full lab in Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E2WRix3C_BtaJYuaWitYtG4aqP9jra5P?usp=sharing)


## 🧠 Background

YOLO (You Only Look Once) is a family of real-time object detection models based on convolutional neural networks (CNNs). YOLOv8, developed by Ultralytics, improves detection accuracy and speed across a variety of applications. In this lab, we apply YOLO to a **socially fraught detection problem** — identifying **homeless camps** from aerial or street-level imagery.

This task raises critical questions:  
- Who defines what is “visible” in the urban landscape?  
- What are the consequences of making certain populations hyper-visible through AI?


## 🧰 Steps for Model Training

### 1. Install YOLOv8

```bash
pip install ultralytics
```

Then in Python:

```python
from ultralytics import YOLO
```

---

### 2. Annotate Training Data

1. Clone the annotation tool:
   ```bash
   git clone https://github.com/HumanSignal/labelImg.git
   cd labelImg
   python -m venv venv
   source venv/bin/activate  # Windows use: venv\Scripts\activate
   pip install pyqt5 lxml
   pyrcc5 -o libs/resources.py resources.qrc
   python labelImg.py
   ```

2. Create bounding boxes for **"camp"** objects representing **homeless camps**. Save the labels in YOLO format.

3. Your dataset structure should look like:

```
homelesscamp_data/
├── images/
│   ├── train/
│   └── val/
└── labels/
    ├── train/
    └── val/
```


### 3. Configure the Dataset

Create a YAML file (`custom_data.yaml`) with the following content:

```yaml
path: /content/dataset/homelesscamp_data
train: images/train
val: images/val
nc: 1
names: ['camp']
```


### 4. Train the Model

```python
model = YOLO('yolov8n.pt')  # Lightweight version
model.train(data='custom_data.yaml', epochs=70, imgsz=640, batch=4)
```

The best-performing weights will be saved in:

```
runs/detect/train/weights/best.pt
```

---

### 5. Run Inference on Test Images

```python
model = YOLO('runs/detect/train/weights/best.pt')
results = model('path_to_test_image.jpg')
results[0].show()
```

Compare results between the **pretrained model** and your **fine-tuned model**.


## ✍️ Written Reflection

At the end of your lab, please respond to **at least two** of the following questions (300–500 words total):

1. How does YOLOv8’s deep learning architecture allow it to detect objects like **homeless camps**?  
2. What are the risks of training AI models to detect socially sensitive features such as **homeless camps**?  
3. What are the potential benefits of such detection? Who might benefit?  
4. What limitations did you notice in how the model performed, either before or after fine-tuning?


## ✅ Deliverables

Your lab submission must include:

1. **Colab Notebook** with detection results from both the pretrained and custom-trained models.
2. **Annotated images** before and after fine-tuning.
3. **Written reflection** (as markdown cell or attached doc/PDF).

Upload your submission to **Canvas** by the due date.

> **Late Policy:** 10% penalty per day unless prior approval granted for valid reasons (illness, emergency, academic conflict).

