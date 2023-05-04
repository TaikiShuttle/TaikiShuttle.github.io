---
layout: project
type: project
image: images/chatgptdetect.png
title: "Machine-Generated Text Detection for ChatGPT"
# All dates must be YYYY-MM-DD format!
date: 2023.01 - 2023.04
projecturl: https://github.com/MGTD4ChatGPT
published: true
labels:
  - NLP
  - Large Language Models
  - Text Classification
summary: "A NLP project trying to classify and analyze machine-generated text."

---

With significant advances in the field of deep learning, large language models (LLM) were used to solve complicated Natural Language Processing (NLP) tasks like natural language understanding and natural language generation. Recently, OpenAI published its newest conversational AI model named ChatGPT. It demonstrates impressive ability in solving all kinds of tasks. However, people are worrying that ChatGPT may be used inappropriately in scenarios like exam-cheating.

In this project, we propose a machine-generated text detector for GPT-3.5. There are three main goals:

1. explore statistical information of machine-generated text (word frequency, text length and sentence structure)
2. build a discriminative model to distinguish machine-generated text and human-written text.
3. propose a data augmentation method to enable the future training of more robust models.



##### Model Construction

We first construct several models trained on Q&A data sets like Narrative Q&A and HC3. We use TF-IDF classifier, Word2Vec&attention classifier and BERT classifier to construct different models. The best performance reaches an AUC score of 0.99. 



##### Data Augmentation

We then combine language patterns observed in analysis with the data and tried to generalize the model to different data set like GPT-wiki data set. We find that adding dependency information may improve the performance of the model. However, we find that models trained on Q&A data set can hardly generated to other scenarios like terminology explanation. Additionally, simply combining the Q&A data set and GPT-wiki data set cannot improve model robustness. Future works should pay more attention on data set construction if a more robust model is expected.



More details can be seen in <a href="../resources/MGTD4ChatGPT.pdf">report</a>.
