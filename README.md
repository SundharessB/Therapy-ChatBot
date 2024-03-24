# Therapy-ChatBot

Welcome to the Therapy Chatbot project! This repository contains code for a therapy chatbot designed to provide supportive and therapeutic responses to user queries. The chatbot utilizes various natural language processing (NLP) techniques and models to generate helpful responses.

# Introduction

This therapy chatbot is designed to provide immediate assistance and support to individuals experiencing suicidal thoughts. Utilizing the advanced capabilities of the `TheBloke/neural-chat-7B-v3-1-GGUF` model, our chatbot aims to engage users in meaningful conversations, offering them guidance and helping to navigate through their crises.

# Objective 

The primary objective of this chatbot is to prevent suicidal attempts by

- Offering a non-judgmental, supportive platform for users to express their feelings.
- Providing timely interventions based on the user's emotional state.
- Alerting designated organizations via email if a user expresses suicidal intent.

# Features

- **Interactive Conversations**: Engages users with empathetic and therapeutic dialogue.
- **Crisis Detection**: Identifies language cues indicative of suicidal ideation.
- **Alert Mechanism**: Automatically notifies support organizations upon detection of high-risk situations.

# How it Works

1. **User Interaction**: Users interact with the chatbot by sharing their thoughts and feelings.
2. **Assistance**: The chatbot provides supportive responses and helps users explore their emotions.
3. **Suicidal Ideation Detection**: If the chatbot detects any indication of suicidal thoughts, it triggers an alert system.
4. **Alerting Organizations**: An email is sent to a pre-determined organization for immediate human intervention.

# Key Packages

1) langchain - Seems to be a custom or specialized library, given the multiple modules imported from it (like vectorstores, embeddings, llms, and chains).
2) transformers - A library by Hugging Face that provides pre-trained models for Natural Language Processing (NLP) tasks like text classification, translation, and more. It includes models like BERT, GPT-2, T5, and others.
3) chainlit - Chainlit is an open-source asynchronous Python framework that enables developers to build scalable Conversational AI or agentic applications quickly and efficiently.

# Install required dependencies

pip install -r requirements.txt

# Requirements

To run this project, you will need the following packages:

- `smtplib`: The standard Python library for sending emails using the Simple Mail Transfer Protocol (SMTP).
- `email`: A package for managing email messages, including `MIMEText` for creating MIME-formatted text emails.
- `langchain_community.document_loaders`: Provides `PyPDFLoader` and `DirectoryLoader` for loading documents into the application.
- `langchain.prompts`: Includes `PromptTemplate` for creating custom prompt templates.
- `langchain_community.embeddings`: Contains `HuggingFaceEmbeddings` for utilizing embedding models from Hugging Face.
- `langchain_community.vectorstores`: Includes `FAISS` for efficient similarity search and clustering of dense vectors.
- `langchain_community.llms`: Contains `CTransformers` for working with transformer models.
- `langchain.chains`: Includes `RetrievalQA` for building retrieval-based question-answering systems.
- `chainlit`: A package for running LangChain applications with ChainLit.

Make sure to install these packages using `pip` before running the project.

# Workflow

This section outlines the workflow of our therapy chatbot, designed to provide support and prevent suicidal attempts. The workflow is divided into several key stages:

### User Interaction
- Users begin by interacting with the chatbot through a conversational interface.
- The chatbot utilizes natural language processing to understand and respond to user inputs.

![Screenshot (117)](https://github.com/SundharessB/Therapy-ChatBot/assets/139948283/ad713001-019d-4442-b5e9-888cfc16df5d)

### Assistance and Support
- The chatbot provides empathetic responses and engages users in therapeutic conversations.
- It offers guidance and support based on the user's expressed emotions and concerns.

![Screenshot (118)](https://github.com/SundharessB/Therapy-ChatBot/assets/139948283/482ce68a-d63f-4fe6-aedf-b84e7e24528d)

### Alert Mechanism

- Upon detecting potential suicidal intent, the chatbot triggers an automated alert system.
- An email notification is sent to a designated organization for immediate human intervention.

![Screenshot (119)](https://github.com/SundharessB/Therapy-ChatBot/assets/139948283/99e59f9c-6a4e-4614-a8b7-7860bcd42b78)


### Follow-Up

- The organization can then reach out to the user to provide further assistance and resources.
- The chatbot also provides information on how to access professional help and emergency services.

### Continuous Improvement

- User interactions are analyzed to improve the chatbot's responses and detection capabilities.
- Feedback loops are established to refine the system and enhance its effectiveness.

# Role of Vector Database

A **Vector Database** is a specialized database designed to store, manage, and index high-dimensional vector data efficiently. These vectors, also known as embeddings, are numerical representations of data objects that carry semantic information.

In our therapy chatbot, the vector database plays a crucial role in understanding and processing user inputs. By converting text into vector embeddings, the chatbot can analyze the conversation's context, detect crisis situations, and provide relevant and personalized support to the user.

The use of a vector database ensures that our chatbot responds with high accuracy and relevance, making it a vital component in our mission to offer timely assistance and prevent suicidal attempts.

This workflow ensures that users receive timely and appropriate support, while also facilitating human intervention when necessary.









