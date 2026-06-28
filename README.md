# 🧠 AdaptiQ – AI-Powered Adaptive Quiz Generator

An intelligent quiz generation platform that automatically creates multiple-choice questions from study materials using Natural Language Processing (NLP), Machine Learning, and OCR. The application supports multiple input formats, predicts question difficulty, and tracks quiz performance for continuous learning.

---

## 🚀 Live Demo

🔗 **Deployed Application:**
**https://your-deployment-url.com**

---

## 📌 Features

* 📄 Generate quizzes from plain text, PDFs, and images
* 🤖 AI-powered question generation using Transformer models
* 📝 Automatic Multiple Choice Question (MCQ) creation
* 🎯 Difficulty prediction (Easy, Medium, Hard)
* 📊 Quiz performance tracking
* 💾 SQLite database for quiz history
* 🔍 OCR support for scanned documents and images
* ⚡ Heuristic fallback when AI models produce insufficient results
* 🌐 Simple and responsive web interface

---

# 🏗️ Project Architecture

```
User
   │
   ▼
Frontend (HTML UI)
   │
   ▼
Flask Backend (app.py)
   │
   ├────────► Document Processor
   │             │
   │             ├── Text Cleaning
   │             ├── PDF Extraction
   │             └── OCR (Images / Scanned PDFs)
   │
   ├────────► Question Generator
   │             │
   │             ├── Transformer Model
   │             └── Heuristic Fallback
   │
   ├────────► Difficulty Classifier
   │             │
   │             ├── ML Model
   │             └── Rule-Based Fallback
   │
   └────────► SQLite Database
                 │
                 ├── Quiz Sessions
                 ├── Scores
                 └── Student Responses
```

---

# 📂 Project Structure

```
Adaptive-Quiz-Generator/
│
├── app.py
├── document_processor.py
├── question_generator.py
├── difficulty_classifier.py
├── database.py
├── adaptiq-premium_fixed (7).html
├── models/
├── static/
├── templates/
├── requirements.txt
└── README.md
```

---

# ⚙️ How It Works

### 1️⃣ Upload Study Material

Users provide learning material in one of the supported formats:

* Plain Text
* PDF Documents
* Images
* Scanned PDFs

---

### 2️⃣ Content Extraction

The application processes the uploaded content by:

* Cleaning plain text
* Extracting text from PDFs
* Performing OCR on images using Hugging Face models

---

### 3️⃣ Question Generation

The extracted content is passed to the AI engine, which:

* Generates question-answer pairs
* Converts them into multiple-choice questions
* Creates meaningful distractor options
* Uses heuristic generation if AI output is insufficient

---

### 4️⃣ Difficulty Prediction

Each generated question is classified as:

* 🟢 Easy
* 🟡 Medium
* 🔴 Hard

using a trained Scikit-learn classifier.

If the classifier model is unavailable, a heuristic based on question complexity is used.

---

### 5️⃣ Quiz Session

The generated quiz is sent to the frontend where users can:

* Answer questions
* View scores
* Check difficulty levels
* Review performance

---

### 6️⃣ Result Storage

After quiz completion, the application stores:

* Quiz Score
* Percentage
* Difficulty Filter
* Input Type
* Student Responses
* Timestamp

using SQLite.

---
# 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.x-000000?logo=flask&logoColor=white)
![Transformers](https://img.shields.io/badge/Transformers-HuggingFace-FFD21E?logo=huggingface&logoColor=black)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-EE4C2C?logo=pytorch&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite&logoColor=white)
![OCR](https://img.shields.io/badge/OCR-Ready-28A745)
![PDF](https://img.shields.io/badge/PDF-Supported-D32F2F)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript&logoColor=black)
---

# 📈 Future Enhancements

* ✅ Adaptive learning based on user performance
* ✅ Personalized quiz recommendations
* ✅ Authentication and user accounts
* ✅ Leaderboard system
* ✅ Cloud database integration
* ✅ Support for DOCX and PPT files
* ✅ Export quizzes as PDF
* ✅ AI-generated explanations for answers
* ✅ Analytics dashboard
* ✅ Multilingual quiz generation

---

# 💻 Installation

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

```
http://127.0.0.1:5000
```

---

# 📸 Screenshots

Add screenshots of:

* Home Page
* Upload Interface
* Generated Quiz
* Difficulty Labels
* Quiz Results
* Performance History

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch

```
git checkout -b feature-name
```

3. Commit your changes

```
git commit -m "Added new feature"
```

4. Push to GitHub

```
git push origin feature-name
```

5. Open a Pull Request

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Your Name**

AI & Full Stack Developer

GitHub: https://github.com/your-username

LinkedIn: https://linkedin.com/in/your-profile

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub!

It helps others discover the project and motivates future improvements.
