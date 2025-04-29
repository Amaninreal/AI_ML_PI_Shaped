# 🩺 Diabetes Prediction using Scikit-learn

This project builds a complete Machine Learning workflow using Scikit-learn to predict whether a patient has diabetes based on input features like age, BMI, blood pressure, etc.

---

## Dataset

- **Source:** [Kaggle - Diabetes Prediction Dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset/data?select=diabetes_prediction_dataset.csv)
- **Features:** Patient medical information (e.g., age, BMI, blood pressure, HbA1c level, etc.)
- **Target:** `diabetes` (0 = No, 1 = Yes)

---

## Project Workflow

### 1. Data Loading & Exploration
- Loaded data using `pandas`.
- Explored the dataset using `.info()`, `.describe()`, and `.head()`.
- Visualized feature correlations using a heatmap (for numerical features only).

### 2. Preprocessing
- Handled missing values if present.
- Applied **Label Encoding** to categorical columns (e.g., `gender`).
- Scaled numerical features using **StandardScaler**.
- Performed an **80/20 Train-Test Split** while maintaining class balance (stratification).

### 3. Model Selection & Building
- Selected **Random Forest Classifier** as the baseline model.
- **Why Random Forest?**
  - It handles both categorical and numerical features effectively.
  - It is robust to outliers and noise.
  - It reduces overfitting by averaging multiple decision trees.
  - It provides **feature importance**, which improves model interpretability.
  - It usually performs well on tabular classification tasks with minimal tuning.

- Built a **Scikit-learn Pipeline** combining preprocessing steps and model training.

### 4. Model Evaluation (Before Tuning)
- Evaluated model performance on the test set using:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1 Score**
- Visualized results with a **Confusion Matrix**.

### 5. Hyperparameter Tuning
- Tuned Random Forest using **GridSearchCV** to optimize:
  - `n_estimators` (number of trees)
  - `max_depth` (tree depth)
  - `min_samples_split` (minimum samples required to split)
- Performed **5-fold cross-validation**, optimizing for **F1 Score**.

### 6. Model Evaluation (After Tuning)
- Evaluated the best model from GridSearchCV.
- Improved metrics across the board.
- Plotted a new **Confusion Matrix**.
- Created a **summary table** comparing Before and After Tuning.

---

## Key Techniques Used

- **Label Encoding** for categorical data.
- **StandardScaler** for feature scaling.
- **Pipeline** to combine preprocessing and model training in one step.
- **GridSearchCV** for hyperparameter tuning with cross-validation.
- **Confusion Matrix** for classification error analysis.
- **Performance Summary Table** for easy comparison.

---