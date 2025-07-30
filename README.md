💡 Customer Churn Prediction Web App
This is a Streamlit-based web application that predicts the likelihood of a customer churning (leaving a service or company), based on various input features. The model is trained using deep learning (TensorFlow/Keras), and uses preprocessing steps such as label encoding, one-hot encoding, and feature scaling.

🚀 How it Works
Model Loading
The trained model is stored in model.h5, and it is loaded using TensorFlow's load_model method.

Encoders and Scaler

label_encoder_gender.pkl: Encodes gender (Male/Female) into numerical format.

onehot_encoder_geo.pkl: One-hot encodes geographical information (e.g., France, Germany, Spain).

scaler.pkl: Standardizes the features to the scale that the model was trained on.

User Input via Streamlit Widgets
The app takes the following input from the user:

Geography: Country of the customer (select box)

Gender: Gender of the customer (select box)

Age: Customer’s age (slider)

Credit Score: Credit score of the customer (number input)

Balance: Account balance (number input)

Estimated Salary: Salary estimation (number input)

Tenure: Number of years the customer has been with the bank (slider)

Number of Products: Number of products they use (slider)

Has Credit Card: Whether they have a credit card (select box)

Is Active Member: Whether they are an active customer (select box)

Data Preprocessing

The inputs are transformed using the loaded encoders and scaler to match the model's expected format.

One-hot encoded geography is concatenated with other features.

All features are scaled using the same StandardScaler used during training.

Prediction

The preprocessed input is fed into the trained neural network.

The model outputs a probability of churn (prediction_proba).

If the churn probability is greater than 0.5, it predicts that the customer is likely to churn.

🧠 Tech Stack
Frontend: Streamlit

Model: TensorFlow/Keras Neural Network

Preprocessing: scikit-learn (LabelEncoder, OneHotEncoder, StandardScaler)

Backend Language: Python

Deployment: Streamlit Cloud / Local

