# 🎫 Automatic Ticket Classification using NLP and Machine Learning

This project aims to automate the customer support ticket system of a financial company using Natural Language Processing (NLP) and Machine Learning (ML) techniques.  
The goal is to accurately identify and categorize support tickets based on their content and assign them to the relevant team for swift resolution.

---

## 🚀 Project Features

- **Automatic ticket classification** using ML models.
- **Real-time ticket classification** using a Streamlit web app.
- **Batch classification** from CSV files for handling multiple tickets at once.
- **Comprehensive documentation** and modular codebase for easy customization.

---

## 🛠️ Technologies Used

- Python
- Natural Language Processing (NLP)
- Machine Learning (Scikit-Learn, XGBoost)
- Streamlit (for Front-end)
- Pandas, NumPy
- Joblib (for model saving/loading)

---

## 🧠 Models and Evaluation

| Model                 | Accuracy | Precision | Recall | F1 Score | ROC AUC Score |
|------------------------|----------|-----------|--------|----------|---------------|
| Logistic Regression    | 0.91     | 0.91      | 0.91   | 0.91     | 0.99          |
| DecisionTreeClassifier | 0.78     | 0.78      | 0.78   | 0.78     | 0.86          |
| RandomForestClassifier | 0.82     | 0.83      | 0.82   | 0.81     | 0.97          |
| MultinomialNB          | 0.71     | 0.74      | 0.71   | 0.67     | 0.94          |
| XGBClassifier          | 0.91     | 0.91      | 0.91   | 0.91     | 0.99          |

✅ Based on performance metrics, **Logistic Regression** and **XGBClassifier** were selected as the best models.

---

## 🧩 Project Structure

```bash
.
├── data/
│   ├── new_tickets.csv         # Example input tickets
│   └── classified_tickets.csv  # Batch classification output
│
├── models/
│   ├── ticket_classifier_model.pkl  # Saved trained model
│   └── vectorizer.pkl               # Saved TF-IDF or CountVectorizer
│
├── scripts/
│   └── batch_classify.py       # Python script for batch classification
│
├── frontend/
│   └── app.py                  # Streamlit app for live ticket classification
│
├── README.md
└── requirements.txt
```

## 🎯 How to Run the Project
1. Clone the Repository
```bash

git clone https://github.com/your-username/automatic-ticket-classification.git
cd automatic-ticket-classification

2. Install Dependencies
```bash

pip install -r requirements.txt
```
3. Run the Streamlit App (Live Manual Entry)
```bash
cd frontend
streamlit run app.py

A web page will open where you can enter ticket text and get the predicted department.
```
4. Run the Batch Classification Script
```bash
cd scripts
python batch_classify.py
```
## 📂 Example Use Cases
- Financial Services (Credit card issues, loan complaints, online banking problems)

- Telecom Industry (Billing, SIM activation, network complaints)

- IT Support Systems (Password reset, access issues, hardware problems)

- E-commerce (Order issues, refund requests, delivery complaints)

## 📌 Future Enhancements
- Integrate Email/Chatbot for real-time ticket intake.

- Multi-label classification (if one ticket fits multiple departments).

- Deploy Streamlit app on Streamlit Cloud / AWS.

- Add AutoML for model selection and hyperparameter tuning.

## 📢 Conclusion
This project streamlines the ticket resolution process, reduces manual effort, improves customer satisfaction, and enables faster response times for IT help desk and customer support teams.
