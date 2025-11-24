📰 Fake News Detection & Credibility Analyzer

A lightweight project that detects whether a news article/headline is Fake or Real, built using Sentence-BERT embeddings, Logistic Regression, LIME explainability, and a Streamlit web app.
Created as part of the GroundTruth AI Internship/Fellowship application.

🚀 Features

SBERT (all-MiniLM-L6-v2) embeddings

Logistic Regression classifier (Accuracy ~96%)

Credibility score (0–100)

LIME explainability → highlights words influencing predictions

Streamlit app for real-time results

Fully reproducible notebook + clean project structure

📂 Project Structure
fake-news-detector/
├── models/
│   ├── classifier.joblib
│   └── sbert_model/        # optional local SBERT model
├── src/
│   └── app_streamlit.py
├── notebooks/
│   └── training_pipeline.ipynb
├── requirements.txt
└── README.md

⚙️ Setup
1. Create virtual environment

Windows

python -m venv venv
venv\Scripts\activate


Mac/Linux

python3 -m venv venv
source venv/bin/activate

2. Install dependencies
pip install -r requirements.txt

3. Add model

Place model file here:

models/classifier.joblib


(Optionally include sbert_model/, otherwise it auto-downloads.)

4. Run Streamlit app
streamlit run src/app_streamlit.py

📊 Evaluation (Summary)

Accuracy: ~96%

Precision/Recall/F1: 95–97%

Confusion matrix & LIME outputs available in the notebook.

🧠 Technical Flow

Text cleaning

SBERT embedding (384-dim)

Logistic Regression classifier

LIMETextExplainer for interpretability

Streamlit UI for predictions

🗂 Dataset

ISOT Fake/Real News Dataset
https://www.kaggle.com/datasets/thought19/fake-news-detector

📜 License

MIT License.

🙋 Author

Aryan Singh
