# Fraud Detection Prediction App

A Machine Learning web application built with **Python** and **Streamlit** that predicts whether a financial transaction is fraudulent based on transaction details.

## Features

- Predicts fraudulent transactions in real time.
- User-friendly Streamlit interface.
- Machine Learning model integrated using Joblib.
- Supports multiple transaction types:
  - PAYMENT
  - TRANSFER
  - CASH_OUT
  - DEPOSIT
- Displays prediction result instantly.

---

## Project Structure

```
Fraud_Detection/
│
├── fraud_detection.py          # Streamlit application
├── fraud_detection_pipeline.pkl # Trained ML model
├── AIML Dataset.csv            # Dataset
├── analysis_model.ipynb        # Model training notebook
├── requirements.txt            # Required packages
└── README.md
```

---

## Technologies Used

- Python
- Streamlit
- Pandas
- Scikit-learn
- Joblib

---

## Dataset Features

The model uses the following input features:

- Transaction Type
- Amount
- Old Balance (Sender)
- New Balance (Sender)
- Old Balance (Receiver)
- New Balance (Receiver)

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Fraud-Detection-Prediction.git
```

Navigate to the project folder:

```bash
cd Fraud-Detection-Prediction
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## Run the Application

Start the Streamlit app:

```bash
streamlit run fraud_detection.py
```

The application will open in your browser at:

```
http://localhost:8501
```

---

## How It Works

1. Select the transaction type.
2. Enter the transaction amount.
3. Enter sender and receiver balances.
4. Click the **Predict** button.
5. The application predicts whether the transaction is:
   - Fraudulent
   - Not Fraudulent

---

## Machine Learning Model

The model was trained using supervised machine learning on a financial transactions dataset.

The trained model is saved as:

```
fraud_detection_pipeline.pkl
```

and loaded into the Streamlit application using Joblib.

---

## Example Output

**Input**

- Transaction Type: PAYMENT
- Amount: 1000
- Sender Balance: 10000
- Receiver Balance: 0

**Prediction**

```
Prediction: Not Fraudulent
```

or

```
Prediction: Fraudulent
```

---

## Future Improvements

- Add transaction time feature.
- Display fraud probability score.
- Upload CSV for batch predictions.
- Deploy using Streamlit Community Cloud.
- Improve model accuracy with hyperparameter tuning.

---

## Author

**Your Name**

GitHub: https://github.com/your-username

LinkedIn: https://linkedin.com/in/your-profile

---

## License

This project is licensed under the MIT License.
