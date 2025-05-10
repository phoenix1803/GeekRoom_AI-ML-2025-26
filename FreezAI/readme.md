# Overview
## Welcome to **FreezAI**, GeekRoom’s very own Kaggle-style Machine Learning competition!  

In this 1-hour challenge, participants will build a predictive model using real-world medical data to determine whether a patient is diabetic.



## Your Objective
Use the given dataset of medical parameters to predict the **Outcome**:
-  `1` =  `Diabetic`  
-  `0` =  `Not Diabetic`


## Allowed Resources
- External help is **allowed** 
  - Google, GitHub, Kaggle Notebooks, LLMs (e.g., ChatGPT, Gemini)  
- Starter notebooks and baselines will be provided



## Task Type
- **Problem**: Binary Classification  
- **Target Variable**: `Outcome`  
- **Evaluation Metric** :  `Accuracy`



Get ready to flex your ML skills in the coolest 60-minute data showdown — **FreezAI**! 

# Description

## 📝 Competition Setup Instructions

1. **Download the Dataset**  
   - Download the `.zip` folder named **freezai** from the competition page.

2. **Unzip the Folder**  
   - Extract the contents of the folder. It contains the following files:
     - `train.csv` – Use this file to train your model.
     - `test.csv` – Use this file to generate predictions.
     - `sample_submission.csv` – Use this as a reference to format your `submission.csv`.

3. **Create a New Kaggle Notebook**  
   - Go to [Kaggle Notebooks](https://www.kaggle.com/code) and create a new notebook under your Kaggle account.

4. **Upload the Files**  
   - Upload the unzipped folder (or the individual files) into your notebook environment.

5. **Train & Predict**  
   - Use `train.csv` to build and train your classification model.
   - Use your trained model to predict outcomes for the samples in `test.csv`.

6. **Create Submission File**  
   - Format your predictions into a file named `submission.csv` with the structure:
     ```
     id,Outcome
     2,0
     5,1
     6,0
     ...
     ```

7. **Submit Your Predictions**  
   - Go back to the competition page and upload your `submission.csv` in the **"Submit Predictions"** section.

---

🔍 **Tip:** Make sure your submission file follows the exact format, and only contains IDs and predicted outcomes (`0` or `1`). Incorrect formatting may result in submission errors.

---

Good luck, and may the coolest model win! ❄️🚀

# Evaluation

Submissions are evaluated based on **Accuracy**, which measures the proportion of correct predictions (0 or 1) compared to the actual `Outcome` values in the test set.

A higher accuracy score indicates a better-performing model. Make sure your model is not only accurate but also generalizes well across unseen data.

---

## Submission Format

Your final submission must be a **CSV file** with the following structure:
    id,Outcome
    2,0
    5,0
    6,0
    etc.


- The `id` corresponds to the ID values provided in the `test.csv` file.
- The `Outcome` should be either `0` (not diabetic) or `1` (diabetic).
- Make sure your file:
  - Includes the header row (`id,Outcome`)
  - Matches the row count of the test set
  - Contains **only integers** (`0` or `1`) — no probabilities

---

⚠️ **Note:** Submissions with incorrect formatting, missing values, or probabilities instead of binary labels may be rejected or scored as 0.

---

Happy modeling and may the most accurate prediction win! 🧊📈

# Dataset Description

## 📂 Files

The following files are provided for this competition:

- **train.csv** — The training dataset. Includes input features along with the target variable `Outcome`.
- **test.csv** — The test dataset. Use this to make predictions. It contains the same features as the training set but without the `Outcome`.
- **sample_submission.csv** — A sample submission file in the correct format (`id,Outcome`) to guide your final submission.


---

## Columns

All files except `sample_submission.csv` contain the following columns:

- `id` — Unique identifier for each individual.
- `Pregnancies` — Number of times the individual has been pregnant.
- `Glucose` — Plasma glucose concentration (mg/dL).
- `BloodPressure` — Diastolic blood pressure (mm Hg).
- `SkinThickness` — Triceps skinfold thickness (mm).
- `Insulin` — 2-Hour serum insulin (mu U/ml).
- `BMI` — Body Mass Index, a measure of body fat based on height and weight:  
- `DiabetesPedigreeFunction` — A function that scores likelihood of diabetes based on family history.
- `Age` — Age of the individual (years).
- `Outcome` — Target variable:  
  - `1` indicates the presence of diabetes  
  - `0` indicates no diabetes

---

## What Are You Predicting?

You are predicting the `Outcome` for each individual in the **test set**. This is a binary classification task where the model determines whether or not a person is likely to have diabetes based on the given features.

---

## Notes

- Make sure your model handles missing or zero values smartly — they might indicate missing data, not true zeroes.
- All numerical columns are continuous, except `Pregnancies` and `Outcome`, which are discrete.

---

