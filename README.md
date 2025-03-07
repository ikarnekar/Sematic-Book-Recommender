# 📚 Semantic Book Recommender with LLMs

This repository contains the complete code for my **Semantic Book Recommender** project. The system leverages **large language models (LLMs)** and **vector search** to provide intelligent book recommendations based on natural language queries.

---

## 🌟 Project Overview

This project consists of five key components:

### 1️⃣ Text Data Cleaning
- **Code:** [`data-exploration.ipynb`](data-exploration.ipynb)
- Prepares and cleans book descriptions to improve recommendation accuracy.

### 2️⃣ Semantic Search & Vector Database
- **Code:** [`vector-search.ipynb`](vector-search.ipynb)
- Uses **vector search** to find books based on user queries (e.g., *"a book about a person seeking revenge"*).

### 3️⃣ Zero-Shot Text Classification
- **Code:** [`text-classification.ipynb`](text-classification.ipynb)
- Classifies books as **fiction** or **non-fiction** to allow filtering.

### 4️⃣ Sentiment Analysis & Emotion Extraction
- **Code:** [`sentiment-analysis.ipynb`](sentiment-analysis.ipynb)
- Determines book tone (e.g., **suspenseful, joyful, sad**) to enhance sorting options.

### 5️⃣ Gradio Web Application
- **Code:** [`gradio-dashboard.py`](gradio-dashboard.py)
- Provides a user-friendly interface for book recommendations.

---

## ⚙️ Installation & Setup

This project was developed with **Python 3.11**. Follow these steps to set up your environment:

### 🔹 1. Install Dependencies
Clone the repository and install dependencies using `requirements.txt`:
```bash
pip install -r requirements.txt
```
Alternatively, install key dependencies manually:
```bash
pip install kagglehub pandas matplotlib seaborn python-dotenv \
    langchain-community langchain-opencv langchain-chroma \
    transformers gradio notebook ipywidgets
```

### 🔹 2. Set Up API Keys
This project requires API keys for **OpenAI** and **Google Books**.

#### 🟢 OpenAI API Key
To create the **vector database**, add your **OpenAI API key** in a `.env` file:
```bash
echo "OPENAI_API_KEY=your_api_key_here" > .env
```

#### 🔵 Google Books API Key
To fetch book data, add your **Google Books API key** in the `.env` file:
```bash
echo "GOOGLE_BOOKS_API_KEY=your_google_books_api_key_here" >> .env
```
You can get a Google Books API key from [Google Cloud Console](https://console.cloud.google.com/).

### 🔹 3. Download the Dataset
The dataset for this project is available on **Kaggle**. Detailed instructions on how to download and use it are provided in the repository.

---

## 🚀 Running the Project
To start the **Gradio web app**, execute the following command:
```bash
python gradio-dashboard.py
```
This will launch a web-based interface for book recommendations.

---

## 🛠 Technologies Used
- **Python** – Data processing & ML workflows
- **Hugging Face Transformers** – LLM-based text embeddings
- **ChromaDB** – Vector search database
- **Gradio** – Interactive UI for book recommendations
- **OpenAI API** – LLM-powered processing
- **Google Books API** – Fetching book details

Feel free to explore and contribute to this project. Happy coding! 🚀📚



