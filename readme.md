# Employee Salary Prediction

This project predicts whether an employee's income is above or below $50K per year using demographic and work-related features. The solution uses machine learning models trained on the Adult Census dataset and provides an interactive web app built with Streamlit.

## Features

- Data cleaning and preprocessing (handling missing values, outlier removal, label encoding)
- Multiple ML models tested (Logistic Regression, Decision Tree, Random Forest, SVM, KNN, Gradient Boosting, AdaBoost)
- Model selection and export using `joblib`
- Streamlit web app for easy predictions with user-friendly input forms
- Encoded categorical variables using label encoding for compatibility with ML models

## How to Run

1. **Install dependencies:**
    ```bash
    pip install pandas scikit-learn matplotlib streamlit joblib
    ```

2. **Train the model:**
    - Run the Jupyter notebook or Python script to preprocess data, train models, and save the best model as `best_model_pipeline.pkl`.

3. **Start the Streamlit app:**
    ```bash
    streamlit run app.py
    ```

4. **Use the App:**
    - Open the provided local URL in your browser.
    - Enter employee details in the form.
    - Get instant salary prediction results.

## Files

- `employeeSalaryPrediction.ipynb` - Main notebook for data processing, model training, and export.
- `app.py` - Streamlit app for interactive predictions.
- `best_model_pipeline.pkl` - Saved best model pipeline.
- `adult 3.csv` - Input dataset (not included, use your own or download from UCI repository).

## Label Encoding Mappings

The app uses the following mappings for categorical variables (must match training):

- **Workclass:** Federal-gov, Local-gov, Others, Private, Self-emp-inc, Self-emp-not-inc, State-gov
- **Marital Status:** Divorced, Married-civ-spouse, Married-spouse-absent, Never-married, Separated, Widowed
- **Gender:** Female, Male
- **Occupation:** Adm-clerical, Craft-repair, Exec-managerial, Farming-fishing, Handlers-cleaners, Machine-op-inspct, Other-service, Priv-house-serv, Prof-specialty, Protective-serv, Sales, Tech-support, Transport-moving, Unknown
- **Relationship:** Husband, Not-in-family, Other-relative, Own-child, Unmarried, Wife
- **Race:** Amer-Indian-Eskimo, Asian-Pac-Islander, Black, Other, White
- **Native Country:** See code for full list

## Author

Created by Abhisek