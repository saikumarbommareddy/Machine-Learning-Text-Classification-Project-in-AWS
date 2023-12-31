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

1. Shervin Minaee [January 4, 2021] “Deep Learning Based Text Classification: A Comprehensive Review” https://arxiv.org/pdf/2004.03705.pdf

   The paper offers an extensive examination of the advancements in text classification achieved through deep learning models compared to traditional machine learning methods. It specifically focuses on diverse applications such as sentiment analysis, news categorization, question answering, and natural language inference. The authors conduct a thorough review of over 150 deep-learning models developed in recent years, delving into their technical contributions, commonalities, and strengths.

   The comprehensive analysis extends to the exploration of more than 40 widely used datasets in the field of text classification, shedding light on the diversity of sources utilized for training and evaluation. Additionally, the paper provides a quantitative assessment of the performance of various deep learning models on popular benchmarks, offering a valuable comparison of their effectiveness.

2. Ameni Bouaziz “Short Text Classification Using Semantic Random Forest” https://www.researchgate.net/profile/Celia-Da-Costa-Pereira/publication/300335247_Short_Text_Classification_Using_Semantic_Random_Forest/links/5cff88474585157d15a225d0/Short-Text-Classification-Using-Semantic-Random-Forest.pdf

   The paper addresses the challenge of using traditional Random Forests for short text classification, revealing a performance decline due to issues such as shortness, sparseness, and lack of contextual information in short texts. The existing solutions to these problems involve data enrichment, but this approach can introduce noise. The authors propose a novel method that combines data enrichment with the integration of semantics into Random Forests.

   In their approach, each short text is enriched with semantically similar data obtained from an external source of knowledge organized into topics using the Latent Dirichlet Allocation model. The learning process in Random Forests is modified to incorporate semantic relations between words during the construction of decision trees. The authors conducted tests on search snippets using their proposed method, demonstrating significant improvements in classification accuracy. The results showed a 34% increase in accuracy compared to traditional Random Forests and a 20% increase compared to MaxEnt. This suggests that incorporating semantic information into the learning process enhances the performance of Random Forests in short text classification tasks.

3. Johnson Kolluri [June 8, 2020]. Text classification using Machine Learning and Deep Learning Models https://deliverypdf.ssrn.com/delivery.php?ID=510070086111087082126117000086016117052035053080091016022066114009095070106099029093043053024038005001055089018069090014013080041021059082052098119121116000031019066036045082066122026083122025076084028117123006017095000071106029025018008122031087024111&EXT=pdf&INDEX=TRUE

   This paper discusses the challenge of dealing with irregular data in various sectors, including universities, businesses, research institutions, technology companies, and government agencies. It emphasizes the importance of organized data for effective analysis and decision-making. Text analytics, translating text into numerical data, plays a crucial role in detecting patterns, and the quality of data organization directly influences the analysis and decision outcomes.

   The manual processing and classification of large datasets are considered difficult, prompting the development of intelligent text-processing tools in the field of Natural Language Processing (NLP). There is a need for automated text classification due to the increasing volume of data and the demand for accuracy. It also identifies a research opportunity in constructing complex text data models using Deep Learning systems, particularly for intricate NLP tasks with semantic requirements. The paper underscores the significance of understanding the nature of data before mining and proposes that data analytics serves as the foundation for text classification. The ultimate goal is to use the results for emergent applications that support decision-making processes, enabling humans to optimize resources and gain maximum benefits.

4. Julliano Trindade Pintas [January 29, 2021]. Feature selection methods for text classification: a systematic literature review. https://www.desirabletomorrows.org/assets/files/GARCIA-A.C.etal.FeatureSelectionMethodsforTextClassification.pdf

   This research paper focuses on the critical role of Feature Selection (FS) methods in improving classification procedures, particularly in the context of text classification. The authors highlight that FS methods are essential for enhancing classification accuracy, reducing data dimensionality, and eliminating irrelevant data. Despite the significance of FS in text classification, the authors note a gap in literature surveys, with few comprehensive analyses available.

   To address this gap, the researchers conducted a Systematic Literature Review (SLR) and came to a two-fold contribution: first, it introduces a new categorization schema for mapping various aspects of each proposed FS method, and second, it provides a detailed mapping of the main characteristics of experiments. These characteristics include the datasets, languages, machine learning algorithms, and validation methods employed in evaluating both new and existing FS techniques. By adhering to the SLR protocol, the authors aim to facilitate the replication of their review process and minimize potential biases in classifying the included studies.

5. Xiaoyu Luo [February 21, 2021]. Efficient English text classification using selected Machine Learning Techniques. https://www.sciencedirect.com/science/article/pii/S1110016821000806?via%3Dihub

   The paper focuses on implementing the Support Vector Machines (SVM) model for classifying English text and documents using text classification. Two analytical experiments were conducted to evaluate selected classifiers with English documents. The experimental results, based on a set of 1033 text documents, indicate that the Rocchio classifier performs well when the feature set is small. However, SVM consistently outperforms other classifiers. The experimental analysis reveals that the classification rate exceeds 90% when the feature set size exceeds 4000 features. Overall, the study highlights the effectiveness of SVM in English text classification, especially when dealing with a larger feature set.


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

  ## AWS Solution Pipeline Chart

![AWS Pipleline_Solution Chart (1)](https://github.com/saikumarbommareddy/CloudComputing/assets/39944794/5c00f027-406b-4567-b8bc-ff99fb6d4967)
