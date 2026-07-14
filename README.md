# 🚀 Briefly – AI-Powered Text Summarizer

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-Transformers-FFD21E?style=for-the-badge)

## 📖 Overview

**Briefly** is an AI-powered web application that generates concise and meaningful summaries from lengthy text using a fine-tuned **T5 Transformer** model.

The application is built using **FastAPI** as the backend framework and a responsive frontend developed with **HTML, CSS, and JavaScript**. It provides users with an intuitive interface where they can paste long text, generate AI-powered summaries in real time, and copy the generated output with a single click.

The project demonstrates the complete deployment pipeline of an NLP model—from preprocessing and inference to REST API development and frontend integration.

---

## ✨ Features

- 🤖 AI-powered abstractive text summarization
- ⚡ High-performance FastAPI backend
- 🎨 Modern glassmorphism-inspired UI
- 📝 Automatic text preprocessing
- 📊 Live character counter
- ⏳ Loading animation during inference
- 📋 One-click copy summary feature
- 💻 Automatic hardware detection (MPS → CUDA → CPU)
- 🔌 REST API for integration with external applications
- 📱 Responsive and clean user interface

---

## 🛠 Tech Stack

### Frontend

- HTML5
- CSS3
- JavaScript

### Backend

- FastAPI
- Pydantic
- Jinja2

### Machine Learning

- Hugging Face Transformers
- PyTorch
- SentencePiece

### Development Tools

- Jupyter Notebook
- Git
- GitHub

---

## 🏗 System Architecture

```text
                 User
                   │
                   ▼
      HTML • CSS • JavaScript
                   │
                   ▼
            FastAPI Backend
                   │
                   ▼
          Text Preprocessing
                   │
                   ▼
             T5 Tokenizer
                   │
                   ▼
      Fine-Tuned T5 Transformer
                   │
                   ▼
         Generated Summary
                   │
                   ▼
          Displayed on Frontend
```

---

## 🔄 Project Workflow

### Step 1 – User Input

The user enters or pastes lengthy text into the application.

### Step 2 – API Request

The frontend sends the input text to the FastAPI backend through a POST request.

### Step 3 – Text Preprocessing

Before inference, the backend cleans the input by:

- Removing HTML tags
- Removing extra spaces
- Removing unnecessary line breaks
- Converting text to lowercase

### Step 4 – Tokenization

The cleaned text is converted into tokens using the T5 tokenizer.

### Step 5 – Summary Generation

The fine-tuned T5 Transformer processes the tokenized input and generates an abstractive summary using beam search decoding.

### Step 6 – Response

The generated tokens are decoded back into readable text and returned to the frontend as a JSON response.

### Step 7 – Output Display

The summary is displayed on the webpage, where users can instantly copy it using the built-in copy button.

---

## 📸 Screenshots

### 🏠 Homepage

![Homepage](screenshots/homepage.png)

---

### ⏳ Summary Generation

![Loading](screenshots/loading.png)

---

### 📋 Generated Summary

![Generated Summary](screenshots/copy-summary.png)

---

## 📂 Project Structure

```text
Briefly/
│
├── screenshots/
│   ├── homepage.png
│   ├── loading.png
│   └── copy-summary.png
│
├── index.html
├── main.py
├── notebook.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🚀 Installation & Setup

Clone the repository

```bash
git clone https://github.com/shubhamm-27/Briefly.git
```

Navigate to the project directory

```bash
cd Briefly
```

Install the required dependencies

```bash
pip install -r requirements.txt
```

Run the FastAPI server

```bash
uvicorn main:app --reload
```

Open your browser

```
http://127.0.0.1:8000
```

---

## ⚙ Model Configuration

| Parameter | Value |
|-----------|-------|
| Model | Fine-Tuned T5 Transformer |
| Framework | Hugging Face Transformers |
| Deep Learning Library | PyTorch |
| Maximum Input Length | 512 Tokens |
| Maximum Output Length | 150 Tokens |
| Beam Search | 4 |
| Early Stopping | Enabled |

---

## 📌 Project Highlights

- Fine-tuned a T5 Transformer model for abstractive text summarization.
- Built a complete FastAPI-based inference pipeline.
- Designed a modern and responsive frontend using HTML, CSS, and JavaScript.
- Implemented automatic text preprocessing before model inference.
- Integrated frontend and backend using REST APIs.
- Added user-friendly features such as loading animation, character counter, and one-click summary copying.

---

## 📌 Note

The trained **T5 model (`saved_summary_model`)** is not included in this repository because of its large size. To run the project locally, place the trained model inside the project directory before starting the FastAPI server.

---

## 🔮 Future Enhancements

- 📄 PDF and DOCX summarization
- 🌍 Multilingual summarization
- 📁 File upload support
- 📊 Adjustable summary length
- 🐳 Docker deployment
- ☁ Cloud deployment
- 🔐 User authentication and summary history

---

## 👨‍💻 Author

**Shubham Sharma**

Aspiring AI Engineer | Machine Learning Enthusiast

📧 Email: shubham789keeds@gmail.com

💼 LinkedIn: [Shubham Sharma](https://www.linkedin.com/in/shubhammm27/)

---
