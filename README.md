# loan-prediction-system
# Loan Prediction System using Machine Learning

## Project Overview

This project predicts whether a loan will be approved or not based on applicant details such as credit score, income, and other features using Machine Learning algorithms.

The model is trained on historical loan data and saved as a serialized file (`model.pkl`) for fast predictions without retraining.


## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib / Seaborn
* Jupyter Notebook

## Dataset

The dataset contains applicant details such as:

* Credit Score
* Income
* Loan Amount
* Other financial attributes


## Features

* Data preprocessing
* Model training (e.g., Naive Bayes / Logistic Regression)
* Model evaluation
* Saved trained model (`model.pkl`)
* Predict loan approval for new inputs

---

##  Model Saving

The trained model is saved using `pickle`:

import pickle
with open("model.pkl", "wb") as f:
    pickle.dump(model, f)


## How to Run

### 1. Clone the repository

git clone https://github.com/your-username/loan-prediction-system.git
cd loan-prediction-system

### 2. Install dependencies

pip install -r requirements.txt


### 3. Run the notebook

jupyter notebook


## Making Predictions

import pickle

with open("model_name.pkl", "rb") as f:
    model_name = pickle.load(f)

# Example input
sample = [[650, 50000, 20000]]

prediction = model.predict(sample)
print(prediction)


## 📷 Output
Naive Bayes model
Prediction on test data [0 0 0 0 0 1 0 0 0 0 0 0 1 0 1 0 0 0 0 1 1 0 1 1 0 0 0 0 0 0 1 0 0 0 0 0 0
 1 0 0 1 0 0 1 1 0 0 0 0 0 0 0 1 0 1 0 0 1 0 0 0 0 0 0 1 1 0 0 0 0 1 1 0 0
 1 0 0 0 1 0 0 1 1 1 0 0 1 0 1 0 0 1 0 0 0 0 0 0 0 0 1 0 0 1 1 0 0 0 0 0 0
 1 0 0 1 0 0 0 1 0 0 0 0 1 0 0 1 1 0 1 0 1 0 0 0 1 0 0 0 0 1 1 1 0 0 0 0 1
 1 0 0 0 0 1 1 0 0 0 0 1 1 1 1 0 0 1 0 0 1 0 1 0 0 0 1 0 1 0 0 0 1 0 0 0 0
 1 1 1 0 0 0 0 0 0 0 0 0 1 0 0]


## Future Improvements

* Deploy using Streamlit
* Add web interface for user input
* Improve model accuracy


## Author

Sonakshi Chauhan
