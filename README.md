# Online Payment Fraud Detection using Machine Learning

## Overview

With the increasing reliance on online payment systems, fraud detection has become a critical concern for financial institutions and payment gateway providers. This project leverages machine learning techniques to detect fraudulent transactions based on transaction details, enhancing the security of online payment systems.

## Features

- **Exploratory Data Analysis (EDA):**
  - Visualizes transaction trends and patterns.
  - Analyzes correlations between different features and fraud occurrences.

- **Machine Learning Models:**
  - Implements Logistic Regression, Random Forest Classifier, and XGBoost Classifier.
  - XGBoost Classifier is identified as the best performer.

- **Model Evaluation:**
  - Uses metrics such as ROC-AUC and Confusion Matrix.
  - Selects the most accurate and generalizable model.

## Dataset

The dataset contains the following features:

- `step`: Time of transaction.
- `type`: Type of transaction (e.g., cash_out, transfer).
- `amount`: Amount transferred.
- `nameOrg`: Sender's account name.
- `oldbalanceOrg`: Sender's balance before the transaction.
- `newbalanceOrg`: Sender's balance after the transaction.
- `nameDest`: Receiver's account name.
- `oldbalanceDest`: Receiver's balance before the transaction.
- `newbalanceDest`: Receiver's balance after the transaction.
- `isFraud`: Target variable (1 for fraudulent, 0 for legitimate).

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/TalariLakshmiNarasimha/Online-Payment-Fraud-Detection-using-Machine-Learning.git
   cd Online-Payment-Fraud-Detection-using-Machine-Learning
   ```

2. (Optional) Set up a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Unix or MacOS
   venv\Scripts\activate     # On Windows
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Place the dataset file (e.g., `transactions.csv`) in the project directory.

2. Run the main script to perform EDA, train models, and evaluate results:
   ```bash
   python main.py
   ```

3. Review the output metrics and plots to analyze model performance.

## Project Structure

```
Online-Payment-Fraud-Detection-using-Machine-Learning/
├── data/                # Dataset files
├── notebooks/           # Jupyter notebooks 
├── requirements.txt     # Python dependencies
├── README.md            # Project documentation
```

## Results

- XGBoost Classifier achieved the highest accuracy and ROC-AUC score among the tested models.
- Key findings and visualization plots are provided in the `notebooks/` directory.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for improvements or bug fixes.

## License

This project is licensed under the MIT License.


