# **GEOG495: Geospatial Artificial Intelligence** 

- **Instructor:** Bo Zhao, zhaobo@uw.edu <img src="res/geoai.png" align="right" width="30%" target="_blank" />  
- **Meeting Time:** Asynchronous 
- **Office Hours:** By appointment or request a zoom meeting via https://t.ly/kpj_t

This course explores the emerging field of Geospatial Artificial Intelligence (GeoAI), focusing on the integration of machine learning, deep learning, and large language models (LLMs) in the context of geographic data. Students will engage both technically and critically with the tools and concepts shaping the future of spatial and placial analysis. This crush course emphasizes hands-on lab experimentation, paper-driven learning, and critical reflection on the social and epistemological implications of AI-powered geospatial technologies.

The class is reading- and lab-driven. Each week begins with a selection of the assigned readings, where students are encouraged to engage with the texts by bringing in real-world examples and critical questions. Lab sessions are guided but self-directed, creating space for open experimentation, problem-solving, and reflective analysis.

## 🧭 Course Objectives

* **Understand** the technical foundations and workflows of GeoAI, including machine learning, deep learning, and LLMs.
* **Apply** open-source tools (Google Colab, GEMINI, ChatGPT API, LangChain) to analyze spatial data.
* **Critically evaluate** the societal, ethical, and epistemological dimensions of AI in geography.
* **Engage with** latest academic literature through weekly readings and reflections.
* **Produce** an independent final essay demonstrating synthesis of technical and critical insights.

> This web page is the syllabus - There is no printed version, please refer here instead. Make sure refer to this page as often as possible. Also, Feel free to ask the instructor for clarifications whenever needed.
---

## 📚 Weekly Schedule

Each week includes ~3 readings, 2 lab sessions and one piece of reading reflection.

### **Week 1: Introduction & Machine Learning for Spatial Data**

We begin with an overview of AI’s evolution and its intersections with geographic thought. Students are introduced to foundational machine learning techniques applied to spatial data using Google Colab. This week sets the tone for the course by situating GeoAI within both technical and critical frameworks.

<details>
<summary><b>Readings</b></summary>

1. Li, W., Arundel, S. T., Gao, S., Goodchild, M. F., Hu, Y., Wang, S., & Zipf, A. (2024). GeoAI for science and the science of GeoAI. Journal of Spatial Information Science, (29), 1–25.
2. Janowicz, K., Sieber, R., & Crampton, J. (2022). GeoAI, counter-AI, and human geography: A conversation. Dialogues in Human Geography, 12(3), 446-458.
3. GeoAI: Machine Learning and Deep Learning with GIS – [GeoWGS84.com](https://www.geowgs84.com/post/geoai-machine-learning-and-deep-learning-with-gis)

> I need to add a reading that focuses on the technical aspects of machine learning, such as a chapter from a machine learning textbook or a relevant research paper
> 4. Burkov, A. (2019). The hundred-page machine learning book. Andriy Burkov. https://themlbook.com

</details>

Lab 1: [Predicting Boston Housing Prices Using Machine Learning](labs/lab01/)

Lab 2: [Downscaling Land Surface Temperature Data of Seattle Using Random Forests](labs/lab02)

### **Week 2: Place, Space and Deep Learning**

This week introduces deep learning architectures for interpreting raster imagery, focusing on CNNs for classification and segmentation. Students also critically reflect on the politics of computer vision, data labeling, and representation in spatial AI.

<details>
<summary><b>Readings</b></summary>

1. Zhao, B., Zhang, S., Xu, C., Sun, Y., & Deng, C. (2021). Deep fake geography? When geospatial data encounter Artificial Intelligence. Cartography and Geographic Information Science, 48(4), 338-352.
2. Lin, Y., & Zhao, B. (2025). Posthuman cartography? Rethinking artificial intelligence, cartographic practices, and reflexivity. Annals of the American Association of Geographers, 115(3), 499-512.

> one reading that focuses on the technical aspects of deep learning, such as a chapter from a deep learning textbook or a relevant research paper
> notes: Bolei Zhou: place recognition, image classification, and segmentation using CNNs
> 2. Li & Ning (2023). *Autonomous GIS: The next-generation AI-powered GIS*. IJDE.
> 1. TorchGeo documentation & tutorial (Microsoft, 2023)

</details>

Lab 3: [Using YOLO to Detect Informal Structures in Urban Spaces](labs/lab03/)

Lab 4: [Geospatial Segmentation with SAM: Deep Learning for Feature Detection](labs/lab04/)


### **Week 3: LLMs for Mapping and Geospatial Reasoning**

This week turns to natural language as a mode of spatial analysis. Students explore how LLMs like ChatGPT can perform geocoding, generate maps, and interpret GIS data from text prompts. Discussions center around the promises and limitations of natural language interfaces.

<details>
<summary><b>Readings</b></summary>

1. Manvi, R., Khanna, S., Mai, G., Burke, M., Lobell, D., & Ermon, S. (2023). GeoLLM: Extracting geospatial knowledge from large language models. arXiv preprint arXiv:2310.06213. https://arxiv.org/abs/2310.06213
2. Peng & Zhao (2024). *Navigating the ethical landscape behind ChatGPT*. Big Data & Society.

> one reading that focuses on the technical aspects of LLMs, such as a chapter from a machine learning textbook or a relevant research paper 
> 3. OpenAI (2023). *ChatGPT: A large language model for conversational AI*. https://openai.com/research/chatgpt
> 4. OpenAI (2023). *ChatGPT API documentation*. https://platform.openai.com/docs/api-reference/chat/create
</details>

Lab 5: [Prompt-to-Map: Using LLMs for Map Generation and Spatial Analysis](labs/lab05)

Lab 6: Natural Language Geocoding – Converting Text to Spatial Data with ChatGPT


### **Week 4: Hallucinations, Bias, and Sustainability**

We conclude by examining the sociotechnical risks of GeoAI. Students critically assess hallucinations, embedded bias, and environmental impacts of AI. The week culminates in an exploratory lab and final reflection.

<details>
<summary><b>Readings</b></summary>

1. Gurnee, W., & Tegmark, M. (2023). Language models represent space and time. arXiv preprint arXiv:2310.02207.
2. Li, P., Yang, J., Islam, M. A., & Ren, S. (2023). Making ai less" thirsty": Uncovering and addressing the secret water footprint of ai models. arXiv preprint arXiv:2304.03271.
3. Gillespie (2024). *Generative AI and the politics of visibility*. Big Data & Society.

</details>

Lab 7: [Critical Exam of GeoAI: Collapse, Hallucination, Bias, and the Limits of Geospatial Intelligence](labs/lab07)

---

## 📜 Course Requirements

###  💻 Computational skill

This course welcomes students who some computational experience, or have programmed in a python or javascript IDE (Integrated Development Environment), especially Google CoLab. Students should at least hear of GIS, GitHub, Leaflet, web crawler, or Raspberry Pi before considering this course, and most importantly, be self-motivated to solve a research question with the listed computational skills.

### 🚀 GitHub

This course material will be hosted on GitHub instead of UW Canvas. On this dedicated GitHub repository for this course, you can find most of the course material, participate in group discussions by submitting GitHub issues, and creating new GitHub repositories to turn in practical exercise deliverables. By the end of this quarter, you will be more proficient in operating a cloud-based coding environment and able to host your work online as a way to gain public and peer attentions.

### 🧾 Quizzes

There will be two short quizzes administered during the course to assess students’ foundational understanding of key technical concepts. These quizzes are designed to reinforce core material covered in lectures, readings, and lab work—such as machine learning workflows, deep learning architectures, spatial data structures, and the capabilities and limitations of large language models in geospatial contexts. The quizzes will be open-note, unlimited time, and may include a mix of multiple choice, short answer, and code interpretation questions. While they are not meant to be high-stakes, the quizzes serve as checkpoints to help students consolidate knowledge and ensure readiness for more advanced lab applications.

### 🧪 Lab Exercises

Students are required to complete eight hands-on lab assignments over the course of four weeks. All labs will be conducted using Google Colab and will focus on applying machine learning, deep learning, and large language models to geospatial data. Each lab involves writing and executing Python code, and students must ensure that their code is clearly organized, well-commented, and reproducible. Final versions of each lab should be submitted via GitHub, along with a short README file explaining the objective, approach, and key outcomes. These labs are designed not only to build technical skills, but also to encourage critical reflection on the design and use of GeoAI methods.

### 👩‍🔬 Reading Reflection

Your weekly think pieces should be at least 350 words in length and should engage critically with the week’s readings**. There is no right or wrong way to write a think piece and you should feel free to experiment, but ensure that you are citing your sources and that your piece is clear and free of any typos. Below are some additional suggestions/guiding thoughts to help shape your piece.

- Though your think piece doesn’t need to follow a formal essay structure, organization, content, and clarity is still important.
- Don’t merely summarize. Develop your own thoughts and reflections in connection to the readings and the lab assignments.
- Lead your reader somewhere beyond the simple observation; in other words, make a point or several points and examine them in depth.
- Use examples and quotations from the assigned text to support what you say. Effective quotations make the piece stronger and more convincing.
- Use this assignment to express more than how you “feel” about the text or problem. Whether you liked the text or not is relevant but should not be the central focus of your think piece.
- Make connections between the assigned text and the course content and above all, explore your own ideas and thoughts about the assigned text; after all, that is the point of the assignment.

### ✍️ Final Essay

The final essay is due at the end of Week 4 and should be between 2,500 and 3,000 words, not exceeding 5,000 words in total. Students are expected to choose a topic related to the course—such as hallucinations in large language models when applied to spatial data, a critical evaluation of GeoAI in disaster response, or the environmental impact of AI models. The essay must incorporate at least two technical sources and two critical sources, either drawn from the course materials or from independent research.

### 📊 Evaluation

| Component               | Weight |
| ----------------------- | ------ |
| Lab Assignments (8)     | 40%    |
| Final Essay             | 25%    |
| Reading Reflections (4) | 25%    |
| Quizzes (2)             | 10%    |


## :notebook_with_decorative_cover: Equity & Inclusivity

Our very highest priorities include creating a brave and supportive class environment where each of us contributes, we can ask big questions, we give and receive critiques in a supportive way, we notice and engage the ways that we are differently situated within past and present relationship of power, privilege and oppression. I invite you to think hard about how race, gender identity, religion, age, citizenship status, first language, ability, sexuality, class, and other axes are at work in our interactions, and what this might mean in terms of when to speak up, when to step back, how to listen, and much more. Each of you is a welcome and invaluable part of our collective whole.

## :love_letter: Disability Accommodations

We welcome the opportunity to work with any students with disabilities in this class to ensure equal access to the course. If you have a letter from Disability Resources for Students (DRS) outlining your academic accommodations, please present the letter to me (or email us, to confirm, if the letter is electronic) as soon as possible so that we can discuss the accommodations you may need for this class. Any discussions between student and professor need to occur as early as possible in order for adequate arrangements to be made. If you do not yet have a letter from DRS, but would like to request academic accommodations due to a disability, please contact DRS [here (Links to an external site.)](https://depts.washington.edu/uwdrs/), or in-person at 011 Mary Gates Hall, or at 206-543-8924 (Voice & Relay), [mailto:uwdrs@uw.edu](mailto:uwdrs@uw.edu).

## :mosque:  Religious Accommodations

Washington state law requires that UW develop a policy for accommodation of student absences or significant hardship due to reasons of faith or conscience, or for organized religious activities. The UW’s policy, including more information about how to request an accommodation, is available at [Religious Accommodations Policy](https://registrar.washington.edu/staffandfaculty/religious-accommodations-policy/). Accommodations must be requested within the first two weeks of this course using the [Religious Accommodations Request form](https://https:/registrar.washington.edu/students/religious-accommodations-request/).

## :memo:  Student Care & Safety

It is important that you take care of yourselves inside and outside of class as you work through stress and other obstacles. There are many different support services on campus that can help, such as the Counseling Center, Hall Health, and the IMA. UW’s Student Care program can help you connect to these and other resources. Learn more an contact them directly: http://depts.washington.edu/livewell/student-care/, livewell@uw.edu, or 206.543.6085. If you are concerned about yourself or a friend who is struggling SafeCampus is a helpful resource. Please add 206.685.7233 to your phones

## :book: Acknowledgement

<a href="https://hgis.uw.edu"><img src="res/logo.png" align="right" width="200px" target="_blank" /></a> This course advocates for the open culture. The course materials are open source for both students and open source community to access. The development of this course was inspired and supported by many generous colleagues and students. I would like to thank Professor Yingjie Hu (University at Buffalo), Professor Lei Zou (Texas A&M University), and Professor Yue Lin (University of Illinois Urbana-Champaign) for their valuable insights. I’m also grateful to Yifan Yang, Haowen Wei, and Haowei Tong who contributed to early explorations with Syllabus and the initial shape of this course during Summer 2024.

`© 2019-2025 All rights are reserved by Bo Zhao.`
