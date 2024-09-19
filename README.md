# Loan Classification Project

## Overview

This project aims to find the best classifier for predicting loan payment status. We use various machine learning algorithms to analyze a dataset of past loans and determine which borrowers are likely to pay off their loans or default.

## Dataset

The dataset (`loan_train.csv`) contains information about 346 customers whose loans have been either paid off or defaulted. It includes the following fields:

- Loan_status: Whether the loan is paid off or in collection
- Principal: Basic principal loan amount
- Terms: Loan repayment schedule (weekly, biweekly, or monthly)
- Effective_date: When the loan was originated
- Due_date: When the loan is due for repayment
- Age: Age of the applicant
- Education: Education level of the applicant
- Gender: Gender of the applicant

## Project Structure

1. Data Loading and Preprocessing
2. Exploratory Data Analysis
3. Feature Engineering
4. Model Training and Evaluation
   - K-Nearest Neighbors (KNN)
   - Decision Tree
   - Support Vector Machine (SVM)
   - Logistic Regression
5. Model Comparison and Selection

## Requirements

- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

You can install the required libraries using:

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/loan-classification-project.git
   cd loan-classification-project
   ```

2. Ensure you have the dataset file `loan_train.csv` in the project directory.

3. Run the Jupyter notebook:
   ```
   jupyter notebook find_the_best_classifier.ipynb
   ```

4. Follow the notebook cells to execute the analysis and model training.

## Results

The project compares four different classifiers:

| Algorithm          | Jaccard | F1-score | LogLoss |
|--------------------|---------|----------|---------|
| KNN                | 0.7037  | 0.82     | NA      |
| Decision Tree      | 0.74    | 0.85     | NA      |
| SVM                | 0.7037  | 0.82     | NA      |
| LogisticRegression | 0.76    | 0.86     | 0.48    |

Based on these results, the Logistic Regression classifier performs the best overall, with the highest Jaccard similarity score and F1-score.


## Contributing

Feel free to fork this project, submit pull requests, or send suggestions to improve the analysis. All contributions are welcome!
