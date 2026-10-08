# Machine Learning-Based Cold-Chain Monitoring and Wastage Risk Prediction

## Project Overview

This project uses Machine Learning to predict the wastage risk category of fresh produce based on storage, processing, inventory, delivery, supplier, and quality-related factors.

The model classifies each record into three wastage risk categories:

- Low
- Medium
- High

## Dataset

The project uses the `fresh_produce_wastage_dataset.csv` dataset.

- Number of records: 3000
- Number of columns: 34
- Target variable: `wastage_risk_category`
- Target classes: Low, Medium, High

## Machine Learning Algorithm

A custom **K-Nearest Neighbors (KNN)** classification algorithm is implemented using Python.

- Learning type: Supervised Learning
- Problem type: Multi-class Classification
- K value: 5

## Technologies Used

- Python
- Pandas
- NumPy
- Joblib
- Jupyter Notebook

## Project Workflow

1. Load the dataset
2. Select relevant features
3. Handle missing values
4. Encode target classes
5. Split data into training and testing sets
6. Perform feature scaling
7. Train the KNN model
8. Generate predictions
9. Evaluate the model
10. Save the trained model using Joblib
11. Load and reuse the saved model

## Project Files

| File | Description |
|------|-------------|
| `fresh_produce_wastage_dataset.csv` | Dataset used for model development |
| `model_development.ipynb` | Notebook for preprocessing, training and evaluation |
| `model_reuse.ipynb` | Notebook for loading and reusing the saved model |
| `wastage_risk_model.joblib` | Saved trained KNN model |

## Model Reuse

The trained model is saved as:

`wastage_risk_model.joblib`

The saved model can be loaded using Joblib and reused to predict the wastage risk category of new records without training the model again.

## Expected Output

The model predicts the wastage risk category as:

**Low / Medium / High**

## Author

Jessica K
