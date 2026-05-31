# Predicting Diabetes with Machine Learning (SVM)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sakshamdubey-byte/diabetes-prediction-svm/blob/main/Diabetes_Prediction_SVM.ipynb)

Hey there! This is a personal machine learning project where I built a Python model to predict whether someone might have diabetes based on their medical stats. 

Since early detection is so important for managing diabetes, I wanted to see how accurately a **Support Vector Machine (SVM)** classifier could spot the patterns in clinical data.

---

## 🗺️ What's Inside?
* [What This Project Does](#-what-this-project-does)
* [The Data I Used](#-the-data-i-used)
* [How I Built It](#-how-i-built-it)
* [How to Run It Yourself](#-how-to-run-it-yourself)
* [Required Packages](#-required-packages)

---

## 🔍 What This Project Does
The main goal here is classification. By looking at a patient's diagnostic measurements, the model figures out whether they are likely to be diabetic or non-diabetic. 

## 📊 The Data I Used
I used the classic **PIMA Indians Diabetes Dataset**, which gives us a few key health metrics to look at:
* **Pregnancies** (Number of times pregnant)
* **Glucose level** (Plasma glucose concentration)
* **Blood Pressure** (Diastolic blood pressure in mm Hg)
* **Skin Thickness** (Triceps skin fold thickness in mm)
* **Insulin level** (2-Hour serum insulin)
* **BMI** (Body Mass Index)
* **Diabetes Pedigree Function** (A score that factors in family history)
* **Age**
* **Outcome** (Our target: `0` means non-diabetic, `1` means diabetic)

## ⚙️ How I Built It
Here’s the step-by-step process I followed in the notebook:
1. **Data Prep:** Loaded up the dataset and did some basic exploratory analysis.
2. **Standardization:** Since these health metrics use completely different scales, I used a scaler to standardize the data so the model treats them fairly.
3. **Splitting:** Split the data into training and testing sets so I could evaluate the model properly.
4. **Training the Model:** Used an SVM Classifier with a linear kernel to train on our data.
5. **Checking Performance:** Evaluated how well the model did by checking its accuracy scores on both the training and test data.
6. **Testing with New Data:** Built a quick predictive system at the end where you can pass in brand-new patient data, and the model will tell you if it predicts diabetes or not.

## 🚀 How to Run It Yourself
If you want to pull this code down and play with it on your local machine, just follow these steps:

1. **Clone this repository:**
   ```bash
   git clone [https://github.com/sakshamdubey-byte/diabetes-prediction-svm.git](https://github.com/sakshamdubey-byte/diabetes-prediction-svm.git)

2.Head into the directory and open up Jupyter Notebook or Google Colab.
3.Open your notebook file and run the cells!

🛠️ Required Packages
Make sure you have these standard data science libraries installed before running the code:

numpy
pandas
scikit-learn

