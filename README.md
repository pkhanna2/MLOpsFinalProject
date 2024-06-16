# Brazilian E-Commerce Customer Satisfaction Prediction

## Overview

This project predicts customer satisfaction in Brazilian e-commerce based on review scores (>=4 or <4) using the [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/olistbr/brazilian-ecommerce/data). The dataset is included in the `ProjectDataset` directory and contains 9 CSV files with a total of 100,000 entries, covering product information, customer details, seller information, and more.

## Notebooks

### 1. FinalProjectCodeMain.ipynb

- **Description**: Utilizes Amazon SageMaker for an end-to-end machine learning pipeline:
  - Exploratory Data Analysis (EDA)
  - Feature Engineering
  - Model Optimization (XGBoost)
  - Model Registration
  - Quality Monitoring and Alarms

### 2. CI CD Implementation.ipynb

- **Description**: Implements Continuous Integration and Continuous Deployment (CI/CD) pipeline for the XGBoost model:
  - **Steps**:
    - Training Step: Trains the XGBoost model using pre-engineered features.
    - Evaluation Step: Evaluates model performance.
    - Condition Step:
      - Fail Step: Executes on model failure.
      - Create Model: Registers the model in the model registry.
      - Register Model: Registers model versions.
      - Transform Step: Performs batch inference.

## Usage

1. **Notebooks**: Execute `FinalProjectCodeMain.ipynb` for model development and monitoring, and `FinalProjectCodeCICD.ipynb` for CI/CD pipeline implementation.

2. **Dataset**: The dataset is provided in the `ProjectDataset` directory. Ensure it's available for the notebooks to access.

3. **Environment**: Python environment should include necessary packages for SageMaker and XGBoost. Consult notebook requirements for specifics.

## Contributors

- Prachi Khanna (pkhanna@sandiego.edu)
- Se'Lina Lasher (slasher@sandiego.edu)
