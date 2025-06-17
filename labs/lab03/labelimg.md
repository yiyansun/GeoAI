
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

#### Installation

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


### 3. Annotate "camp" Objects

Once LabelImg is open and running, follow these steps to label your images for training:

1. **Open the image directory**  
   Click on the folder icon or use the `Open Dir` button to navigate to your training image folder (e.g., `images/train/`).

2. **Select YOLO format**  
   In the bottom-right corner, ensure that the output format is set to **YOLO**. This ensures that the label files are written in the correct format expected by YOLOv8.

3. **Begin labeling each image**  
   For each image:
   - Use your mouse to draw a bounding box around any visible **homeless camp structure**, such as a tent, tarp, shelter, or informal enclosure.
   - Avoid labeling unrelated items (e.g., cars, poles, people) unless they are part of the structure.
   - Try to include the entire object within the bounding box, without excess background.

4. **Enter the class name**  
   When prompted, type in the class name exactly as: `camp`.  
   If it’s your first time using this name, LabelImg will register it in memory.

5. **Save the label**  
   Click the save icon or press `Ctrl + S` to save your annotations. LabelImg will create a `.txt` file in the same folder structure, containing bounding box info in YOLO format.

6. **Repeat for all training images**  
   Continue labeling the rest of your images, one by one. You can use the arrow keys or navigation bar to move between images efficiently.


Each saved label file will contain lines like:

```
15 0.543 0.674 0.225 0.310
```

Where:
- `15` is the class index for `camp` (if other default classes exist, `camp` is often added as class 15)
- The remaining numbers are normalized values:
  - `x_center`, `y_center`, `width`, `height`
  - All are relative to the image dimensions, ranging from 0 to 1

> **Tip:** Double-check that your saved `.txt` label files match your images by name (e.g., `01.jpg` ↔ `01.txt`) and are stored in the corresponding `labels/train/` or `labels/val/` folder.


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

By following this process, you will have created a full YOLO-compatible dataset for detecting homeless camps in real-world imagery.