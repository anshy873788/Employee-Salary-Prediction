# Employee Income Prediction Project

This project aims to build and evaluate machine learning models to predict whether an individual's annual income is above or below 50K based on demographic and employment data.

## Dataset

The project uses the "Adult Income" dataset, which contains various features about individuals, such as age, workclass, education level, marital status, occupation, relationship, race, gender, capital gain, capital loss, hours per week, and native country. The target variable is 'income', which is categorized as '<=50K' or '>50K'.

## Project Steps

The following steps were performed in this notebook:

1.  **Data Loading:** The dataset was loaded into a pandas DataFrame.
2.  **Data Cleaning and Preprocessing:**
    *   Handled missing values, specifically replacing '?' with 'others' or 'NotListed' in relevant columns ('occupation', 'workclass').
    *   Removed specific categories from 'workclass' ('Without-pay', 'Never-worked').
    *   Removed lower education levels.
    *   Dropped the original 'education' column.
    *   Filtered the data to include ages between 18 and 75.
    *   Categorical features were label encoded.
    *   Numerical features were scaled using `MinMaxScaler`.
3.  **Data Splitting:** The dataset was split into training and testing sets.
4.  **Model Training and Evaluation:** Five different classification models were trained and evaluated on the preprocessed data:
    *   K-Nearest Neighbors (KNN)
    *   Logistic Regression
    *   Random Forest Classifier
    *   Gradient Boosting Classifier
    *   Support Vector Classifier (SVC)
    Accuracy and classification reports were generated for each model.
5.  **Model Comparison:** The accuracy of the trained models was visualized using a bar chart.

## Model Performance

The notebook includes the accuracy scores and detailed classification reports for each model, allowing for a comparison of their performance in predicting income levels. The bar chart provides a visual summary of the accuracy comparison.

## How to Run the Code

1.  Upload the `adult 3.csv` dataset to your Google Drive.
2.  Open this notebook in Google Colab.
3.  Ensure your Google Drive is mounted (run the cell with `drive.mount`).
4.  Run all the code cells sequentially from top to bottom to load the data, perform preprocessing, train the models, and view the results and visualizations.

## Libraries Used

*   pandas
*   numpy (often used implicitly by pandas and scikit-learn)
*   sklearn (for preprocessing, model selection, and models)
*   matplotlib (for visualization)
