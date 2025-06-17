
## Training Dataset Creation Using LabelImg

To train YOLOv8 on a custom class like `"camp"`, you first need to create a labeled dataset. This file explains how to collect images, install the annotation tool, create bounding boxes, and structure your dataset for training.

### 1. Download Images

The source images in this lab were manually collected from **Google Street View** and other open web sources. We focused on locations where **homeless camps** are visible.

You can save screenshots or download images with recognizable structures like tents, tarps, or shelters in urban settings. Be sure to keep the image filenames informative, such as encoding geographic coordinates:

```
47.6019764%2C-122.3306162.jpg
```

> **Note:** Try to capture a diversity of angles, lighting, and object scales for robust training.

### 2. Install and Launch LabelImg

LabelImg is a lightweight, open-source tool for manual image annotation. You can install it on your laptop or desktop following the instruction below.

#### Installation (Mac/Linux/Colab VM)

```bash
# Clone the tool
git clone https://github.com/HumanSignal/labelImg.git
cd labelImg

# Set up Python environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install pyqt5 lxml
pyrcc5 -o libs/resources.py resources.qrc

# Launch LabelImg
python labelImg.py
```

If the instruction does not work, please follow the instruction on the front page of LabelImg's GitHub Repository: https://github.com/HumanSignal/labelImg .


### 📐 3. Annotate "camp" Objects

Once LabelImg is open:

1. Open the image folder (e.g., `images/train/`)
2. Choose **YOLO** as the output format (bottom-right selector)
3. Draw bounding boxes around homeless camps (tents, structures, etc.)
4. Enter the class name exactly as `camp`
5. Save the annotations (LabelImg will create `.txt` files in YOLO format)

💡 Each saved label file will contain lines like:

```
15 0.543 0.674 0.225 0.310
```

Where:
- `15` is the class index for `camp`  
- Remaining values are normalized `x_center y_center width height`

If LabelImg shows multiple class names (e.g., default classes 0–14), your `camp` class may be assigned as class `15`.

---

### 4. Organize the Dataset

After labeling:

```
homelesscamp_data/
├── images/
│   ├── train/        ← Your training images
│   └── val/          ← Manually split a few images here for validation
└── labels/
    ├── train/        ← Auto-saved label files from LabelImg
    └── val/          ← Copy matching label files for validation images
```

Ensure each image in `images/train/` has a matching `.txt` file in `labels/train/`.

---

### 5. Zip the Dataset

Once your folder structure is complete, compress the root directory:

```bash
zip -r homelesscamp_data.zip homelesscamp_data/
```

This ZIP file can now be uploaded to Google Colab and used for YOLOv8 training via:

```python
model.train(data='path/to/custom_data.yaml', ...)
```

✅ By following this process, you will have created a full YOLO-compatible dataset for detecting homeless camps in real-world imagery.