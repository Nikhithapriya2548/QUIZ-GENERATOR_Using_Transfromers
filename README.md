# 🧠 AdaptiQ – AI-Powered Adaptive Quiz Generator

> Transform your study materials into intelligent, adaptive quizzes using Artificial Intelligence.

AdaptiQ is an AI-powered web application that automatically generates multiple-choice quizzes from study materials. It leverages Natural Language Processing (NLP), Machine Learning, and OCR to extract content, create meaningful questions, classify their difficulty, and track learning progress.

---

## ✨ Features

* 🤖 AI-generated Multiple Choice Questions (MCQs)
* 📄 Supports Plain Text, PDF, and Image uploads
* 🔍 OCR for scanned documents and handwritten notes
* 🎯 Automatic difficulty classification (Easy • Medium • Hard)
* 📊 Quiz scoring and performance analytics
* 💾 SQLite database for storing quiz history
* ⚡ Smart fallback question generation when AI confidence is low
* 🌐 Responsive and user-friendly interface

---

## 🏗️ System Overview

```text
Study Material
      │
      ▼
Content Extraction
      │
      ▼
AI Question Generation
      │
      ▼
Difficulty Prediction
      │
      ▼
Interactive Quiz
      │
      ▼
Performance Tracking
```

---

## 📂 Project Structure

```text
Adaptive-Quiz-Generator/
│
├── app.py                      # Flask application
├── document_processor.py       # Text extraction & OCR
├── question_generator.py       # AI-based MCQ generation
├── difficulty_classifier.py    # Difficulty prediction
├── database.py                 # SQLite database operations
├── templates/                  # HTML templates
├── static/                     # CSS, JavaScript & Assets
├── models/                     # Trained ML models
├── requirements.txt
└── README.md
```

---

## ⚙️ How It Works

### 📥 1. Upload Study Material

Upload learning content in one of the supported formats:

* Text
* PDF
* Images
* Scanned Documents

### 🔍 2. Content Processing

The application extracts and cleans the uploaded content using text extraction and OCR techniques.

### 🤖 3. AI Question Generation

Transformer-based models generate question-answer pairs and convert them into multiple-choice questions. If necessary, a heuristic engine ensures high-quality quiz generation.

### 🎯 4. Difficulty Classification

Each question is classified into one of three levels:

* 🟢 Easy
* 🟡 Medium
* 🔴 Hard

using a trained Machine Learning model or a rule-based fallback.

### 📈 5. Quiz & Performance Tracking

Users answer the generated quiz, receive instant feedback, and their quiz history is securely stored for future review.

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend

* Python
* Flask

### Artificial Intelligence

* Hugging Face Transformers
* Scikit-learn
* OCR Models
* NLP Techniques

### Database

* SQLite

### Libraries

* Transformers
* PyTorch
* pdfplumber
* Pillow
* pytesseract
* scikit-learn

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/adaptive-quiz-generator.git
```

Navigate into the project

```bash
cd adaptive-quiz-generator
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

Open your browser

```text
http://127.0.0.1:5000
```

---

## 📸 Application Preview

> Add screenshots of:

* 🏠 Home Page
* 📄 Upload Interface
* ❓ Generated Quiz
* 📊 Quiz Results
* 📈 Performance History

---

## 🌱 Future Enhancements

* 👤 User Authentication
* ☁️ Cloud Database Integration
* 📚 Personalized Learning Paths
* 🌍 Multi-language Quiz Generation
* 📥 Export Quizzes as PDF
* 🧠 AI-generated Answer Explanations
* 📊 Advanced Learning Analytics
* 🏆 Leaderboards & Achievements

---

## 🤝 Contributing

Contributions are always welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👩‍💻 Author

**Your Name**

AI | Machine Learning | Full Stack Developer

📧 [your-email@example.com](mailto:your-email@example.com)

🌐 GitHub: https://github.com/your-username

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star!

**"Learning becomes smarter when AI meets education."**

</div>
