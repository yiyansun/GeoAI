# Critical Exam of GeoAI: Collapse, Hallucination, Bias, and the Limits of Geospatial Intelligence

- **Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); 
- **Teaching Assistant:** Liz Peng, lp36@uw.edu
- **Points Available** = 10

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

Some of the earliest concepts were inspired by insightful conversations with Dr. Yue Lin.