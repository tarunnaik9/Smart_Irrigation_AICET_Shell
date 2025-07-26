# Smart_Irrigation_AICET_Shell
This is AICET Internship Cycle 2


#  Smart Irrigation System – AICET Internship Cycle 2

This project is developed as part of **AICET Internship Cycle 2** under the title **Smart Irrigation System**.  
The goal is to automate irrigation decisions using machine learning based on environmental and crop-related data, helping optimize water usage and improve agricultural efficiency.

---

##  Project Objective

To predict whether irrigation is required based on:
- Temperature
- Humidity
- Soil Moisture
- Soil Type
- Crop Type

The system uses a **Decision Tree Classifier** trained on a dataset to make predictions and displays results in a user-friendly format.

---

##  Steps Followed

###  STEP 1: LOAD AND PREPROCESS DATA
- Loaded `irrigation_machine.csv` dataset using `pandas`.
- Checked for missing/null values.
- Applied **Label Encoding** to categorical features:
  - `Soil Type`
  - `Crop Type`

###  STEP 2: DEFINE FEATURES AND LABELS
- Selected input features:
  - `Temperature`, `Humidity`, `Moisture`, `Soil Type`, `Crop Type`
- Target variable: `Irrigation` (0 = Not Required, 1 = Required)

###  STEP 3: TRAIN-TEST SPLIT
- Split the dataset using `train_test_split()`:
  - 80% Training
  - 20% Testing

###  STEP 4: TRAIN CLASSIFIER
- Used **DecisionTreeClassifier** from `sklearn`.
- Trained the model using the training dataset.

###  STEP 5: EVALUATE MODEL
- Predicted on test data.
- Evaluated the model using:
  - Accuracy Score
  - Classification Report
  - Confusion Matrix
- Displayed test results in a clean format simulating a dashboard.

---

##  Files Included

- `Irrigation_System.ipynb` – Jupyter Notebook with code for data loading, preprocessing, training, and evaluation.
- `irrigation_machine.csv` – Dataset containing environmental and crop data.

---

##  Technologies Used

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

