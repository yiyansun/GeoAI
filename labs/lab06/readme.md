# Prompting Geospatial Reasoning: Understanding Space and Place with Gemini

- **Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); 
- **Teaching Assistant:** Liz Peng, lp36@uw.edu
- **Points Available** = 10

This lab explores how large language models (LLMs)—specifically Google Gemini—can be prompted to extract geospatial and semantic information from narrative texts. You will analyze a walking tour chapter of Seattle's Capitol Hill and generate structured location data that includes not only names and coordinates, but also cultural and emotional attributes such as sense of place and rhetorical framing.

By comparing LLM outputs with traditional geocoding methods, you will assess how well Gemini “understands” both spatial structure and placial meaning. This lab combines prompt engineering, mapping, and critical reflection on AI’s ability to interpret geography.

You will:

- Design a structured prompt to extract 16 features from a narrative PDF
- Run Gemini Flash 2.0, Gemma, and Gemini 2.5 Preview to compare model behavior
- Parse model output and visualize on an interactive Folium map
- Reconstruct the same map using traditional geocoding (ArcGIS) from a manually curated CSV
- Compare results in terms of location accuracy and semantic richness
- Reflect on how prompt structure affects geospatial reasoning and place interpretation

> **Guiding question:** How does prompt engineering shape an LLM’s ability to "read" geography and understand place?

Click this button to launch the full lab on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1doYON6zQdHYLzKtmXbR_1ORskl0CIM-W?usp=sharing)

### Coding Experiments

Extend your analysis by adding the following experiments as new code blocks in your notebook:

- Revise the prompt (e.g., remove fields or examples). How does Gemini respond?
- Compare outputs from different models. Which performs best, and why?
- Analyze map error: Which locations are misrepresented, and what might explain this?

### Written Reflection

At the end of your lab, please answer **at least two** of the following questions (300–500 words total):

1. How does prompt specificity affect the quality of spatial extraction?
2. In what ways does Gemini succeed or fail in expressing "sense of place"?
3. How does LLM-based mapping differ from rule-based geocoding?
4. What are the implications of letting LLMs narrate geography?

---

## ✅ Deliverables

All deliverables must be submitted via **Canvas Discussion Board**, under the thread corresponding to this lab. Your Canvas post for this lab should look like:

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
