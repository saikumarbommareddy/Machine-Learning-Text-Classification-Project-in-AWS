# Cloud Computing - Group 07

## Group Members:
- Juhi Jadhav
- Sai Kumar Reddy Bommareddy
- Apoorve Bhargava
- Soumik Paul
- Raj Kumar

## Data Source:

https://www.kaggle.com/competitions/llm-detect-ai-generated-text/data 

## Project Scope: 

This project's machine learning component attempts to solve the problem of telling student essays from essays produced by large language models (LLMs). The main objective is to create a model that can reliably determine if an essay falls into the LLM-generated category (1) or the student-written category (0). By using machine learning techniques for text classification, this activity is in line with the goals of the AWS Academy Cloud Foundations and Data Engineering teaching programs.

## Domain:

This research is focused on natural language processing and education. The essays in the dataset were written by students and produced by LLMs in response to particular stimuli. It is essential to comprehend the essential elements of the education domain, such as the variety of student writing styles and the possible modifications brought about by LLMs. One of the potential challenges could be separating authentic student expression from stuff generated by a machine.

Educators: The model's accuracy can aid educators in assessing the authenticity of student work, providing insights into potential instances of plagiarism or automated content generation.
Students: Ensuring fair evaluation and recognition of genuine student effort is in the interest of the students.
Developers/Researchers: Those involved in the development of large language models or educational technologies can benefit from insights into the distinguishing features of student and LLM-generated essays.


## Literature Review:

The paper offers an extensive examination of the advancements in text classification achieved through deep learning models compared to traditional machine learning methods. It specifically focuses on diverse applications such as sentiment analysis, news categorization, question answering, and natural language inference. The authors conduct a thorough review of over 150 deep-learning models developed in recent years, delving into their technical contributions, commonalities, and strengths.

The comprehensive analysis extends to the exploration of more than 40 widely used datasets in the field of text classification, shedding light on the diversity of sources utilized for training and evaluation. Additionally, the paper provides a quantitative assessment of the performance of various deep learning models on popular benchmarks, offering a valuable comparison of their effectiveness.

Shervin Minaee [January 4, 2021] “Deep Learning Based Text Classification: A Comprehensive Review” https://arxiv.org/pdf/2004.03705.pdf

The paper addresses the challenge of using traditional Random Forests for short text classification, revealing a performance decline due to issues such as shortness, sparseness, and lack of contextual information in short texts. The existing solutions to these problems involve data enrichment, but this approach can introduce noise. The authors propose a novel method that combines data enrichment with the integration of semantics into Random Forests.

In their approach, each short text is enriched with semantically similar data obtained from an external source of knowledge organized into topics using the Latent Dirichlet Allocation model. The learning process in Random Forests is modified to incorporate semantic relations between words during the construction of decision trees. The authors conducted tests on search snippets using their proposed method, demonstrating significant improvements in classification accuracy. The results showed a 34% increase in accuracy compared to traditional Random Forests and a 20% increase compared to MaxEnt. This suggests that incorporating semantic information into the learning process enhances the performance of Random Forests in short text classification tasks.

Ameni Bouaziz “Short Text Classification Using Semantic Random Forest” https://www.researchgate.net/profile/Celia-Da-Costa-Pereira/publication/300335247_Short_Text_Classification_Using_Semantic_Random_Forest/links/5cff88474585157d15a225d0/Short-Text-Classification-Using-Semantic-Random-Forest.pdf



## Domain-specific Challenges:

1. Ethical Considerations:
- Fair evaluation: It is essential to guarantee the fairness of the evaluation procedure. It is not acceptable for the model to inadvertently discriminate against or favour particular student groups on the basis of things like writing style or language ability.
- Detection of plagiarism: It takes careful balancing to address the moral conundrum of reliably recognising information generated by machines without violating student privacy.

2. Regulations and Privacy:
- Protecting Student Data: It is critical to follow laws governing the usage and security of student data. In order to prevent sensitive data from being misused or accessed without authorization, the model should be created with privacy in mind.

3. Interpretability:
- Explainability: The model's predictions might need to be explained to educators and other stakeholders. Building trust and comprehending the decision-making process depend on the model's interpretability.

4. Bias in Language Models:
- Bias Mitigation: Big language models could unintentionally reinforce biases found in their training sets. Fair evaluations require addressing and reducing biases in the model's predictions.

## KPI’s:

1. Accuracy:
- Total Accurate Predictions: It is essential to accurately categorize essays as either LLM-generated or student-written. A high accuracy rate suggests that the model is good at differentiating between the two groups.

2. Precision:
- Real Benefits Among Expected Benefits: To evaluate the model's capacity to distinguish between essays produced by LLMs and those authored by students accurately, precision is essential. Low false positives are indicated by a high precision score.

3. Recall:
- Verified Advantages Among Real Advantages: In order to include all LLM-generated essays in the dataset, recall is crucial. High recall guarantees that LLM-generated information is recognized by the model.

4. F1-Score:
- Verified Advantages Among Real Advantages: In order to include all LLM-generated essays in the dataset, recall is crucial. High recall guarantees that LLM-generated information is recognized by the model.

5. Fairness Metrics:
- Harmonic Average of Accuracy and Memory: Precision and recall are measured in a balanced manner by the F1-Score. When there is a disparity between the quantity of essays produced by LLMs and students, it is very helpful.

6. Interpretability Metrics:
  - Explanatory Power: To guarantee openness and reliability, metrics pertaining to the model's interpretability, such as offering justifications for forecasts, are crucial.

