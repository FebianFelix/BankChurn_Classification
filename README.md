# BankChurn_Classification

This project uses machine learning models, specifically Decision Tree and Random Forest classifiers, to predict customer churn for a hypothetical bank. By understanding customer churn, the bank can devise better strategies to retain clients and enhance customer satisfaction.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Data Preparation](#data-preparation)
- [Modeling](#modeling)
- [Evaluation Metrics](#evaluation-metrics)
- [Results and Findings](#results-and-findings)
- [Installation](#installation)
- [Usage](#usage)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project focuses on predicting customer churn using supervised machine learning techniques. The goal is to identify key features that influence churn behavior in the banking industry, allowing the bank to reduce churn rates through targeted interventions.

## Dataset

- **Source**: A dataset obtained from Kaggle, representing customer data for the fictional bank.
- **Features**:
  - **Credit Score**: Reflects customer creditworthiness.
  - **Geography**: Customer location (e.g., country).
  - **Gender**: Customer gender.
  - **Age**: Customer’s age.
  - **Tenure**: Duration of customer relationship with the bank.
  - **Balance**: Bank balance of the customer.
  - **Num of Products**: Number of products a customer has.
  - **Has Credit Card**: Indicator if the customer owns a credit card.
  - **Is Active Member**: Whether the customer is actively using bank services.
  - **Estimated Salary**: Customer’s estimated annual income.
  - **Exited**: Target variable indicating churn (1 if churned, 0 if retained).

## Technologies Used

- **Python** for data processing and model training.
- **Jupyter Notebook** for data analysis and visualization.
- **scikit-learn** for machine learning models.
- **Matplotlib** and **Seaborn** for data visualization.

## Data Preparation

1. **Data Cleaning**: Ensured no missing values and removed unnecessary columns.
2. **Encoding**: Encoded categorical variables such as 'Geography' and 'Gender' for model compatibility.
3. **Outlier Detection and Removal**: Identified and handled outliers in key features to improve model accuracy.
4. **Normalization**: Scaled numeric features to improve model performance.

## Modeling

The following models were used for classification:
1. **Decision Tree Classifier**: A basic tree-based model for classification.
2. **Random Forest Classifier**: An ensemble model that uses multiple decision trees to improve prediction accuracy and reduce overfitting.

Both models were trained and evaluated using key performance metrics, and cross-validation was applied to ensure the reliability of model results.

## Evaluation Metrics

- **Accuracy**: The percentage of correct predictions.
- **Precision** and **Recall**: Used to assess the quality of churn predictions, especially for classifying customers likely to churn.
- **F1-Score**: Provides a balance between precision and recall.
- **Confusion Matrix**: To visualize prediction errors and accurately evaluate model performance.

## Results and Findings

- **Random Forest** outperformed Decision Tree in overall accuracy and demonstrated a higher F1-Score and recall for the churn class.
- **Key Features Influencing Churn**: Age, Credit Score, and Balance were identified as major factors that correlate with customer churn.
- **Cross-Validation Results**: Random Forest achieved consistent accuracy across multiple validation folds, reinforcing its effectiveness in predicting churn.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/FebianFelix/BankChurn_Classification.git
   ```
2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

## Usage

1. Load the Jupyter Notebook files and run each cell to execute the data preparation, EDA, modeling, and evaluation steps.
2. Use the `RandomForestClassifier` and `DecisionTreeClassifier` sections to analyze feature importance and evaluate model performance on the test set.

## Conclusion

The analysis highlighted that Random Forest is more robust in handling the complexities of predicting customer churn. The project provided insights into the demographic and financial characteristics of customers who are more likely to churn, enabling better-targeted retention strategies.

## Contributing

1. **Fork the repository**.
2. **Create a branch** for your feature (`git checkout -b feature/AmazingFeature`).
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`).
4. **Push to the branch** (`git push origin feature/AmazingFeature`).
5. **Open a Pull Request**.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
