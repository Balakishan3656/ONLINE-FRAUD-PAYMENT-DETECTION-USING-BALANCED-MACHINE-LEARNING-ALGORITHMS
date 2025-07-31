# ONLINE-FRAUD-PAYMENT-DETECTION-USING-BALANCED-MACHINE-LEARNING-ALGORITHMS

This project is a Django web application for detecting fraudulent online transactions using machine learning models such as Random Forest and Naive Bayes. It also employs SMOTE for handling imbalanced datasets and provides visual insights into model performance.

## Features

- Upload and process transaction datasets
- Predict fraudulent transactions from uploaded data
- Train and evaluate ML models (Random Forest, Naive Bayes)
- Use SMOTE for data balancing
- Visualize metrics and confusion matrix using Matplotlib and Seaborn
- User registration and login functionality

---

## Project Structure

```bash
├── FraudApp/
│   ├── static/
│   ├── templates/
│   │   ├── index.html
│   │   ├── Predict.html
│   │   ├── Register.html
│   │   ├── UserLogin.html
│   │   └── UserScreen.html
│   ├── views.py  # Main logic
├── Dataset/
│   └── PS_20174392719_1491204439457_log.csv
├── model/
│   └── data.npy  # Preprocessed train-test split data
├── manage.py
└── README.md
```

---

## Technologies Used

- **Backend:** Django (Python)
- **ML Models:** Random Forest, Naive Bayes
- **Data Handling:** Pandas, NumPy, SMOTE
- **Visualization:** Matplotlib, Seaborn
- **Database:** MySQL (via PyMySQL)
- **Frontend:** HTML templates rendered by Django

---

## Machine Learning Workflow

1. Load dataset and encode categorical features.
2. Split into training and testing sets.
3. Apply SMOTE for balancing imbalanced classes.
4. Train:
   - Random Forest
   - Naive Bayes
   - Random Forest with SMOTE
   - Naive Bayes with SMOTE
5. Evaluate using:
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - Confusion Matrix

---

## How to Run

1. **Clone the repo**
   ```bash
   git clone https://github.com/Balakishan3656/fraud-detection-app.git
   cd fraud-detection-app
   ```

2. **Set up Python environment**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run MySQL and create a database**
   ```sql
   CREATE DATABASE fraud;
   ```

4. **Launch the server**
   ```bash
   python manage.py runserver
   ```

5. **Access the app**
   Visit `http://127.0.0.1:8000/` in your browser.

---

## Screens and Actions

- **Home:** Welcome screen
- **Register/Login:** User authentication
- **Load Dataset:** View summary of fraud data
- **Train Models:** View algorithm accuracy, precision, recall, F1
- **Balanced Data:** Visualize data balance after SMOTE
- **Prediction:** Upload transaction CSV and see results

---

## Sample Visualizations

- Confusion Matrix
- Bar chart comparison of ML algorithms (Accuracy, Precision, Recall, F1)

---

## Requirements

```txt
Django
pandas
numpy
matplotlib
seaborn
scikit-learn
imblearn
pymysql
```

---

## License

This project is for academic and educational use only.
