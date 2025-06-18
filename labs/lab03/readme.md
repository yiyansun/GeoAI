# Identifying Homeless Camps Using YOLO

- **Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); 
- **Teaching Assistant:** Liz Peng, lp36@uw.edu
- **Points Available** = 10

This lab introduces students to object detection using YOLOv8, a state-of-the-art deep learning framework for visual recognition. We apply this tool to a socially sensitive use case: identifying homeless camps from Google Street View imagery. In doing so, students will engage not only with advanced AI workflows but also with critical questions about surveillance, social visibility, and ethical deployment of geospatial technologies.

The project blends technical practice with reflective thinking: students train a custom model, compare detection performance, and critically examine the societal implications of automating visibility.

You will:

* Use a pretrained YOLOv8 model to perform object detection
* Annotate street-level imagery using LabelImg and generate a YOLO-compatible dataset
* Train a custom YOLOv8 model to recognize “camp” structures
* Visualize and compare detection results before and after training
* Map predictions by extracting GPS coordinates from filenames
* Reflect on the consequences of using deep learning to identify vulnerable populations

> **Guiding question:** What does it mean to automate the detection of social marginality?

Click this button to launch the full lab on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E2WRix3C_BtaJYuaWitYtG4aqP9jra5P)

### Coding Experiments:

Extend your analysis by adding the following experiments as new code blocks in your notebook:

- Adjust the number of training epochs, batch size, or input image resolution. Observe how these changes affect training accuracy and validation performance.
- Experiment with adding more annotated training samples to your dataset. Does increasing the diversity or quantity improve detection quality?
- Try testing your model on new Google Street View images from different locations within Seattle. Does the model generalize across neighborhoods or city districts?

### Written Reflection:

At the end of your lab, please answer **at least two** of the following prompts (300–500 words total):

1. What differences did you observe between pretrained and fine-tuned detection?
2. How well does your trained model generalize to new images or unseen parts of Seattle?
3. What changes occurred when you added or replaced training data? Did performance improve?
4. What are the key limitations and opportunities of using deep learning in this task?
5. What ethical concerns arise from using AI to detect homeless encampments?
6. If detection data were published or integrated into public platforms (e.g., OpenStreetMap), what impact might that have on real communities?

---

## ✅ Deliverables

All deliverables must be submitted via **Canvas Discussion Board**, under the thread corresponding to this lab . Your Canvas post for this lab should look like:

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

This lab is built upon Zeen Lin's early contribution, and later Miaomiao Li helped me explore the functions of Yolo and created the training dataset.