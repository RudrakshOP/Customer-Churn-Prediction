🔮 Customer Churn Prediction App

A simple yet powerful Streamlit web application that predicts whether a customer is likely to churn based on demographic and account information. Built using TensorFlow, scikit-learn, and Streamlit.


🚀 Live Demo
🔗 https://iucmtzyawm6ofs5tubc9vh.streamlit.app/


📌 Overview
This app uses a pre-trained deep learning model to estimate customer churn probability. The model was trained on structured banking data and uses the following techniques:

🌐 One-Hot Encoding for Geography
⚙️ Label Encoding for Gender
📊 Standard Scaling for numerical features
🤖 Neural Network built with TensorFlow/Keras
📉 Outputs churn probability score
✅ Fully interactive via Streamlit UI

Features:
Input customer attributes such as age, balance, credit score, etc.
Real-time churn prediction with user-friendly interface
Output includes:
Churn Probability (0 to 1)
Final prediction (Churn or Not)


🛠️ Tech Stack
Frontend: Streamlit
Backend: Python
Model: TensorFlow / Keras
Preprocessing: scikit-learn (LabelEncoder, OneHotEncoder, StandardScaler)
Deployment: Streamlit Cloud

📁 Project Structure
graphql
Copy
Edit
├── app.py                      # Streamlit application
├── model.h5                    # Trained Keras model
├── label_encoder_gender.pkl    # Label encoder for Gender
├── onehot_encoder_geo.pkl      # One-hot encoder for Geography
├── scaler.pkl                  # StandardScaler for feature scaling
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation

