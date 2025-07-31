# -LegalQA-AI-Powered-Legal-Document-Analysis-System
# 📜 LegalQA: AI-Powered Legal Document Clause & Risk Analyzer

![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0db7ed?style=for-the-badge&logo=docker&logoColor=white)

A professional-grade AI system that automatically extracts legal clauses, classifies risk levels, and visualizes insights from contracts using NLP and machine learning.

---

## 🚀 Features

- ✅ **Multi-Format Support**: PDF, DOCX, TXT, Excel, and JSON
- ✅ **Clause Risk Scoring**: ML-based classification (High / Medium / Low)
- ✅ **Keyword Extraction**: Highlight legal entities and patterns
- ✅ **Streamlit Web App**: Clean and responsive dashboard
- ✅ **CSV/Excel Export**: One-click clause download for review
- ✅ **Modular Codebase**: Clear separation of UI, logic, and ML models
- ✅ **Docker-Ready**: Instant deployment with `docker build & run`

---

## 🧠 ML Model Overview

| Component              | Details                                |
|------------------------|----------------------------------------|
| Model                  | Logistic Regression (TF-IDF features)  |
| Dataset                | Sample 20–100 legal clauses (CUAD-ready) |
| Features               | N-grams (1–3), clause length, keywords |
| Output                 | Risk Level: High / Medium / Low        |
| Export Format          | CSV, Excel, JSON                       |

> 🔁 Roadmap includes BERT / InstructorXL upgrade & clause-level anomaly detection.

---

## 📊 Architecture

```mermaid
graph TD
    A[Upload Legal Contract] --> B[File Parser (PDF/DOCX)]
    B --> C[Text Chunking & Clause Detection]
    C --> D[Risk Classifier (ML)]
    C --> E[Keyword / Entity Highlighter]
    D --> G[Streamlit UI Results]
    E --> G
    G --> H[Export as CSV/Excel/JSON]
🛠️ Installation
1️⃣ Clone the repo
bash
Copy
Edit
git clone https://github.com/yourusername/LegalQA.git
cd LegalQA
2️⃣ Create virtual environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
3️⃣ Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
🧪 Run the App
▶️ Start the Streamlit Web UI
bash
Copy
Edit
streamlit run legal_qa_app.py
Visit: http://localhost:8501

🐳 Run with Docker
bash
Copy
Edit
docker build -t legalqa .
docker run -p 8501:8501 legalqa
📂 Folder Structure
php
Copy
Edit
LegalQA/
├── app/                # Core application logic
│   ├── ui.py
│   ├── processor.py
│   ├── risk_model.py
│   └── file_handler.py
├── models/             # Trained models & vectorizers
│   └── risk_classifier.pkl
├── data/               # Sample contracts & training data
├── outputs/            # Exported clause results
├── tests/              # Unit tests
├── static/             # Logos, assets, demo GIF
├── legal_qa_app.py     # Streamlit app entry point
├── requirements.txt
├── Dockerfile
├── README.md
└── LICENSE
📈 Sample Output
Clause Title	Risk Level	Key Phrases
Termination Clause	High	termination, breach
Payment Obligation	Medium	payment, invoice

🚧 Future Enhancements
 ⚙️ BERT / InstructorXL clause encoder

 🔍 OCR + OpenCV support for scanned contracts

 📎 CUAD-based training pipeline

 🧠 Risk anomaly detection (Isolation Forest / AE)

 🔐 User authentication for multi-user dashboards

 🏗️ Hugging Face Spaces deployment

 📚 Streamlit + LangChain fallback QA chatbot

🤝 Contributing
Fork the project

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📜 License
Distributed under the MIT License. See LICENSE for details.

✨ Maintainer
Muhammad Mashood Iqbal
Trainee Data Scientist | Open Source Contributor | LegalTech AI Enthusiast
