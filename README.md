# Supplier News Categorization

This repository contains the code and datasets for developing a **Supplier News Categorization System**. The system classifies news articles into predefined categories: **Geopolitical, Finance, Natural Disasters, and Regulatory**. It leverages advanced **NLP techniques**, including topic modeling and classification using **BERT-based embeddings**.

---

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Future Enhancements](#future-enhancements)
- [Acknowledgments](#acknowledgments)

---

## Overview

The Supplier News Categorization system is designed to process and classify real-time supplier-related news articles. The system utilizes:

- **Text Preprocessing**: Cleans and tokenizes text data for modeling.
- **Topic Modeling**: Utilizes LSI, LDA, and **BERTopic** for topic discovery and classification.
- **Real-time Updates**: Ensures articles are categorized as they are received, allowing stakeholders to address supplier risks **proactively**. 

This system aims to provide stakeholders with actionable insights to address supplier risks efficiently.

---

## Project Structure

├── README.md # Project documentation
├── SupplierNewsCategorization_Part1.ipynb # Data preprocessing and topic modeling
├── SupplierNewsCategorization_Deployment.ipynb # Deployment pipeline
├── newsdata.csv # Raw dataset of 2000+ news articles
├── classified_documents_with_topics.csv # Results with assigned topic labels

---

## Key Features

- **Preprocessing Pipeline**: Text cleaning, tokenization, and lemmatization for optimal analysis.
- **Topic Modeling**: BERT-based embedding for precise classification with relevant seed keywords.
- **User-Friendly Outputs**: Structured outputs with tokens, topic labels, and probabilities for each article.

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/Supplier-News-Categorization.git](https://github.com/yourusername/Supplier-News-Categorization.git)
   cd Supplier-News-Categorization
2. Install Dependencies:
   ```bash
   pip install -r requirements.txt
3.Download the pretrained BERT base uncased model and place it in the repository directory.
4.Open the Jupyter Notebooks to explore the implementation:
   SupplierNewsCategorization_Part1.ipynb: Contains data preprocessing and topic modeling steps.
   SupplierNewsCategorization_Deployment.ipynb: Used to simulate deployment for real-time categorization.


## Usage
### Run the Preprocessing Notebook:
Open SupplierNewsCategorization_Part1.ipynb to clean the raw dataset and perform topic modeling. This notebook includes:
Text cleaning (removal of special characters and stopwords)
Tokenization and lemmatization
Topic modeling using BERT-based embeddings with seed keywords

### Deploy the System:
Use SupplierNewsCategorization_Deployment.ipynb to simulate the deployment process for real-time categorization. This will:
Categorize new supplier news articles using the preprocessed data.
Store the results, including topic labels and probabilities, in classified_documents_with_topics.csv.

## Future Enhancements
Real-Time Web Dashboard: Integrate the system into a web dashboard or app widget for dynamic, real-time categorization of supplier news articles.
Multilingual Support: Add support for non-English articles, enabling global applicability.
Model Improvement: Enhance classification accuracy by fine-tuning transformer models for better understanding and categorization of complex topics.

## Acknowledgments
Hugging Face Transformers: For providing pre-trained transformer models, including BERT-based embeddings.
Beautiful Soup: For web scraping and extracting relevant data from news articles.
BERTopic: For topic modeling and visualization of results.
