# Ford Car Price Prediction

## Project Description
This project analyzes used Ford car listings and builds Linear Regression models to estimate car prices from vehicle attributes. It demonstrates exploratory data analysis, feature preparation, categorical encoding, scaling, model training, and regression evaluation.

## Objectives
- Explore the Ford car dataset and understand its features.
- Prepare numeric and categorical variables for modelling.
- Train a Linear Regression model.
- Compare different approaches for encoding categorical features.

## Tools and Technologies
- Python
- Jupyter Notebook
- NumPy and Pandas
- Matplotlib and Seaborn
- Scikit-learn

## Dataset
The notebook loads a file named `ford.csv`. The workflow references vehicle features such as:
- Model
- Year
- Mileage
- Tax
- MPG
- Engine size
- Transmission
- Fuel type

The target is the car price column in the dataset.

## Workflow
1. Load `ford.csv`.
2. Inspect and explore the dataset.
3. Separate input features from the price target.
4. Encode categorical columns using alternative approaches.
5. Scale selected numerical features in one approach.
6. Split the data into training and test sets.
7. Train Linear Regression models.
8. Compare the models using regression metrics.

## Repository Structure
```text
ford-car-price-prediction/
├── README.md
├── requirements.txt
├── project of ml from start to end .ipynb
└── ford.csv                 # Include only if redistribution is permitted
```

## How to Run
1. Install Python 3.10 or newer.
2. Clone or download this repository.
3. Place `ford.csv` in the same folder as the notebook.
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Start Jupyter:
   ```bash
   jupyter notebook
   ```
6. Open the notebook and run the cells from top to bottom.

## Evaluation
The notebook imports MAE, MSE, and R² metrics. Run the notebook and record the final MAE, RMSE, and R² values here so readers can compare model performance. RMSE can be calculated as the square root of MSE.

## Important Notes
- The dataset file must be named exactly `ford.csv` unless the notebook path is updated.
- The notebook compares encoding approaches; use the same train/test split when comparing models fairly.
- Fit preprocessing transformations on the training set only. A scikit-learn `Pipeline` and `ColumnTransformer` are recommended to prevent data leakage.
- Label encoding nominal categories can incorrectly imply an order. One-hot encoding is generally more appropriate for categories such as transmission and fuel type.

## Learning Outcomes
- Understand a regression workflow.
- Prepare mixed numeric and categorical data.
- Compare encoding strategies.
- Interpret common regression metrics.

## Disclaimer
This is an educational project. Predictions are estimates and should not be treated as guaranteed market prices.
