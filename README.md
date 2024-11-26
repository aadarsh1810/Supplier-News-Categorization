# Supplier News Categorization System

This repository contains the implementation of a Supplier News Categorization system using NLP and LLM (Large Language Model)-based techniques. The system classifies supplier-related news articles into four categories:

1. **Finance**
2. **Geopolitical**
3. **Regulatory**
4. **Natural Disasters**

The objective is to help businesses analyze supplier-related news in real time for better risk assessment and decision-making.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

The Supplier News Categorization system processes real-time or historical supplier news articles and assigns them to predefined categories using a combination of:
- Pre-trained sentence transformers (`all-MiniLM-L6-v2` for topic embeddings).
- Custom category embeddings and similarity-based mapping.

This system automates the tedious task of reading and categorizing supplier news, enabling quick and efficient identification of risks or opportunities in the supply chain.

---

## Features

- **Flexible Categorization**: Supports dynamic news categorization with LLM-based topic embeddings.
- **Real-Time Analysis**: Enables real-time categorization of incoming news articles.
- **Customizable Categories**: Easily extendable to more categories based on business needs.
- **High Accuracy**: Utilizes sentence transformers and cosine similarity for precise mappings.

---

## Dataset

- The dataset contains columns such as:
  - **Date**: Publication date of the article.
  - **Title**: Title of the news article.
  - **Content**: Full text of the news article.
  - **Topic Label**: Labels generated using LDA/BERTTopic techniques.
  - **Predicted Category**: Final mapped category based on similarity scoring.

### Class Distribution
| Category          | Count |
|-------------------|-------|
| Geopolitical      | 445   |
| Finance           | 264   |
| Regulatory        | 215   |
| Natural Disasters | 84    |

---

## Installation

### Prerequisites

- Python 3.7+
- Google Colab or local environment with GPU support.
- Required Python libraries:
  - `sentence-transformers`
  - `pandas`
  - `torch`
  - `scikit-learn`

