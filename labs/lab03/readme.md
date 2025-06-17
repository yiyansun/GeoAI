# Identifying Homeless Camps Using YOLO

**Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); **Points Available** = 50

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

Try one or more of the following in your notebook:

* Run inference using the pretrained YOLOv8n model. What does it detect?
* Fine-tune your model using custom “camp” annotations. Compare the results.
* Adjust the number of epochs, batch size, or input image resolution. How does performance change?
* Visualize prediction results on an interactive map using Folium.
* Try predicting on new Street View locations not in the training set.



### Written Reflection:

At the end of your lab, please answer **at least two** of the following prompts (300–500 words total):

1. What differences did you observe between pretrained and fine-tuned detection?
2. How well can your trained model generalize to new contexts?
3. What are the key limitations and opportunities of using deep learning in this task?
4. What ethical concerns arise from detecting homeless encampments with AI?
5. How would public mapping of these features—e.g., via OpenStreetMap—impact real people?


## ✅ Deliverables

Your submission must include **two parts**:

1. **Coding Experiments:** Annotated code cells, results, and map visualizations.
2. **Written Reflection:** A short critical write-up based on the questions above.

Please export both parts into a **Word document or PDF** and upload to **Canvas**.

**Note:** Lab assignments must be submitted electronically to Canvas by the due date. Late submissions will incur a 10% penalty per day unless prior notice is given for valid reasons such as illness, academic conflicts, or personal emergencies. Flexibility is possible with timely communication, but make-up exams or extensions will only be granted in documented, exceptional cases.