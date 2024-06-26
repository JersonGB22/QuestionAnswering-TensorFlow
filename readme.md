# <h1 align="center">**Question Answering**</h1>

<p align="center">
<img src="images/image_readme.png"> 
</p>

This repository implements Question Answering models, a natural language processing (NLP) task that retrieves the answer to a question from a given text. These models are created using the TensorFlow and Hugging Face Transformers libraries. There are two types of this task:

1. **Extractive:** Extracts the answer directly from the provided context.
2. **Abstractive:** Generates a correct answer freely based on the context or without it.

## **Common Use Cases:**
- **Virtual Assistants:** Answering user questions using information from a specific database.
- **Document Search:** Finding precise answers in large document sets.
- **Customer Service:** Providing quick and accurate responses to customer inquiries.
- **Education:** Helping students get answers to questions based on study materials.

## **Implemented Models:**

- **Extractive Model for Answerable Questions:** This RoBERTa Large model has been fine-tuned with the [Stanford Question Answering Dataset (SQuAD)](https://huggingface.co/datasets/rajpurkar/squad) to appropriately answer questions within a given context. SQuAD consists of 100,000 question-answer pairs across more than 500 Wikipedia articles, where the answer is a text segment from the corresponding passage. The model has achieved an excellent **F1 Score** of **94.1%** on the validation set.

- **Extractive Model for Answerable and Unanswerable Questions:** This model is a more robust and challenging version of the previous one, fine-tuned with [SQuAD 2.0](https://huggingface.co/datasets/rajpurkar/squad_v2) to appropriately answer both answerable and unanswerable questions within the provided context. SQuAD 2.0 consists of the 100,000 question-answer pairs from SQuAD plus 50,000 unanswerable questions. The model is capable of responding to questions within the context and also returns ``No Answer`` if the answer is not in the context or if it is of an abstractive type. It has achieved an excellent **F1 Score** of **87.7%** on the validation set.

## **Some Results**

<p align="left">
<img src="images/images_models/prediction_qa_val_2.png" style="width: 1249px;"> 
</p>

---
<p align="left">
<img src="images/images_models/prediction_qa_val_1.png" style="width: 1238px;"> 
</p>

---
<p align="left">
<img src="images/images_models/prediction_qa_matrix.png" style="width: 1366px;"> 
</p>

---
<p align="left">
<img src="images/images_models/prediction_qa_worldwar2.png" style="width: 1366px;"> 
</p>

#### *Further results can be found in their respective notebooks.*

## **Technological Stack**
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white&labelColor=101010)](https://docs.python.org/3/) 
[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white&labelColor=101010)](https://www.tensorflow.org/api_docs)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=white&labelColor=101010)](https://huggingface.co/)
[![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white&labelColor=101010)](https://plotly.com/)

## **Contact**
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&labelColor=101010)](mailto:jerson.gimenesbeltran@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=101010)](https://www.linkedin.com/in/jerson-gimenes-beltran/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=101010)](https://github.com/JersonGB22/)