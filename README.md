# Asking Clarifying Questions

This is NLP-Spring 23, IIT KGP term project.

This problem statement deals with asking clarifying questions in open-domain dialogue systems. This allows for obtaining any additional information that may give more context to the conversation. This is enabled by solving the following 2 subtasks:

1. When to ask a clarifying question: Given an instruction, does it require a clarifying question to be asked? This can be seen as a binary classification problem. The label ‘1’ would indicate a need for asking a clarifying question while‘0’ would indicate the opposite. The evaluation metric used in this case is the macro average F1 score.
2. Which clarification question to ask: Given an instruction, the model has to rank a list of clarifying questions according to their relevance. The evaluation metric to be used is Mean Reciprocal Rank (MRR).

Dataset and Starter Code: [](https://github.com/aliannejadi/ClariQ:)[https://github.com/aliannejadi/ClariQ](https://github.com/aliannejadi/ClariQ)

## Team Details

Name: Transformers

Members

* 19CS10020 - Bhushan Malani
* 19CS10034 - Harshit Jindal
* 19CS10039 - Kaushal Banthia
* 19CS10068 - Jayant PSY

## Setup Instructions

### Classification Task

[Notebook](./Clarification_Need_Prediction.ipynb) - [Colab Link](https://colab.research.google.com/drive/1lGPXNyUvyplTEltofE6fDP0QOrFR61p2)

Connect Drive to store the finetuined classification model.

Run all the cells to get desired output.(Comments and other instructions are added at appropriate places in the notebook)

### Question Relevance Task

[Notebook](./clariq_baseline_bert_based.ipynb) - [Colab Link](https://colab.research.google.com/drive/1m-gneeMlwS3AMuBosvcFCLB1grvC-Rlw#scrollTo=sDPJh2oX_i4G)

Change the drive location of stored models in the notebook(by default "/content/drive/MyDrive/NLP").

Change the CLASSIFICATION_MODEL and RANKER_MODEL varibale as per requirement.

To get results with classifier uncomment the 2nd cell in 'Training a transformer-ranker for ClariQ (RQ2)' subsection, to set CLASSIFICATION_MODEL to None

Else keep it commented.

Run all the cells to get results
