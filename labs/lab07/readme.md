# Critical Exam of GeoAI: Collapse, Hallucination, Bias, and the Limits of Geospatial Intelligence

**Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); **Points Available** = 10

This lab offers a critical and technical investigation into the spatial reasoning capacities and failures of large language models (LLMs), using Gemini to geocode addresses in Seattle. Students will analyze how hallucinations, semantic collapse, and social biases emerge through LLM-generated g deospatial data, and reflect on the epistemological limits of AI-powered spatial intelligence.

You will:

- Sample real address data from OpenStreetMap and generate geocoded predictions using Gemini
- Compute and visualize spatial error, identifying patterns of hallucination and collapse
- Investigate the precision of LLM outputs and how they affect geocoding reliability
- Enrich spatial data with U.S. Census variables (e.g., income, race, broadband, education)
- Train a Random Forest model to analyze predictors of spatial error
- Reflect critically on bias, visibility, and what GeoAI does or doesn’t see

> **Guiding question:** What does GeoAI “know” about space — and whose geographies are most likely to be collapsed, hallucinated, or hidden?

Click this button to launch the full lab on Colab: [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vPi72aGdr-eAXvSuNIBDj4dJHIV0jAW7)

---

## Coding Experiments:

Try one or more of the following extensions in your notebook:

- Use one of the pre-generated datasets with 500 or 1000 address points. Does more data reduce collapse or bias?
- Swap in a different LLM (e.g., GPT-4o via ChatGPT API) for address prediction. Do errors and collapse patterns shift?
- Repeat the same workflow in another city (e.g., Portland, Chicago, or Atlanta). Are results similar or different?
- Remove precision-limited predictions (e.g., with fewer than 3 decimal places) and assess the impact on overall error.

## Written Reflection:

At the end of your lab, please answer **at least two** of the following prompts (300–500 words total):

1. Where did the LLM perform well — and where did it fail most significantly?
2. What kinds of places were most likely to be collapsed into others? What might explain this?
3. How did social and geographic features (e.g., income, race, location) correlate with model error?
4. What limits of GeoAI did this lab help you surface — technical, social, ethical, or otherwise?
5. What would a more just or equitable geocoding model look like?

## ✅ Deliverables

Your submission must include **two parts**:

1. **Notebook Experiments:** Add your own testing (e.g., larger datasets, model changes, visualizations) and generate any relevant plots or outputs.
2. **Written Reflection:** Submit a short reflection responding to the prompts above.

Please export both parts into a **PDF or Word document** and upload it to **Canvas**.

**Note:** Lab assignments must be submitted electronically to Canvas by the due date. Late submissions will incur a 10% penalty per day unless prior notice is given for valid reasons such as illness, academic conflicts, or personal emergencies. Flexibility is possible with timely communication, but make-up exams or extensions will only be granted in documented, exceptional cases.

#### Acknowledgement

Some of the earliest concepts were inspired by insightful conversations with Dr. Yue Lin.