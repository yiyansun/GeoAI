# Prompt-to-Map: Using LLMs for Map Generation and Spatial Analysis

- **Instructor:** Bo Zhao, [zhaobo@uw.edu](mailto:zhaobo@uw.edu); 
- **Teaching Assistant:** Liz Peng, lp36@uw.edu
- **Points Available** = 10

This lab introduces students to a novel geospatial workflow where **large language models (LLMs)** serve as natural language interfaces for map creation and spatial analysis. Instead of coding from scratch, students write **textual prompts** that guide the AI to generate code, extract spatial data, and interpret geospatial patterns.  

This lab blends **hands-on machine learning** with **critical GIS reflection**, encouraging students to not only experiment with prompt engineering and map automation, but also question what it means to “delegate” spatial reasoning to AI.

You will:

* Use natural language to prompt spatial workflows (e.g., geocoding, mapping, modeling)
* Retrieve and visualize real-world data (coffee shops, census income)
* Perform spatial joins and basic statistical modeling
* Evaluate how LLMs interpret geographic tasks
* Reflect on prompt design, bias, and the limits of automation in geography

> **Guiding question:** In what ways can prompting with natural language help us create clearer, more accurate maps?

Launch the lab notebook on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1UT5quBP02HyDvj89FCJ0AjibEM1deSxT#scrollTo=LlvzfSYFvo8-)

---

### Prompt-Based Experiments

Try one of the following prompt explorations:

* Change the point of interest (e.g., from coffee shops to public parks).
* Modify the spatial unit (e.g., use ZIP codes instead of Census tracts).
* Use a vague or minimalist prompt—what gets left out or misinterpreted?
* Ask the model to explain its own output or errors in plain English.

---

### ✍Written Reflection

At the end of your lab, please respond to **at least two** of the following questions (300–500 words total):

1. How did the specificity of your prompt influence the quality of code or analysis?
2. What parts of the spatial workflow did the LLM handle well—and where did it fail?
3. In what ways does this approach change how you understand GIS or cartographic design?
4. What are the social or epistemological risks of relying on LLMs for spatial analysis?

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