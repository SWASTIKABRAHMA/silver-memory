1. Dataset Description
The dataset used in this project was loaded from an Excel file containing columns with various unnamed entries. The target variable for analysis was set as Unnamed: 2, which underwent cleaning and preprocessing. The dataset contained significant missing values, particularly in the target column.

Key details:

>Initial structure: Multiple unnamed columns with missing entries.
>Target column: Identified as Unnamed: 2.
>Features: Other columns excluding the target variable.

2. Preprocessing Steps
To prepare the dataset for analysis, the following steps were performed:

  1.Check Missing Values:
   
   >Identified rows in the target column with missing values.

  2.Handle Missing Data:

   >Dropped rows with missing target values where necessary.
   >Reconstructed the feature (X) and target (y) variables post-cleaning.
   >Applied mean imputation for the remaining missing target values.
  
  3.Feature-Target Splitting:

   >Features (X): Columns except the target column.
   >Target (y): Column Unnamed: 2.

3. Setting Up the Environment
Ensure the following packages are installed to run the project:

bash
pip install pandas scikit-learn openpyxl

1.Clone or Download the Project:

  >Save the notebook , script locally or use GitHub.
  >Ensure the dataset file (LUSID Excel - Setting up your market data (1).xlsx) is in the appropriate directory.

2.Prepare Python Environment:

   >Use Python 3.7 or later.
   >Install necessary libraries listed above.

3.Run the Code:

   >Execute the script in a Jupyter Notebook or Colab environment.

4. Models Used
   Two machine learning models were implemented and evaluated:

   1.Linear Regression:

    >Used for initial prediction trials.
    >Evaluation Metrics:
    >Mean Absolute Error (MAE)
    >Mean Squared Error (MSE)
    >R² Score
    
   2.Random Forest Regressor:

    >Applied to enhance predictive capabilities.
    >Results:
    >MAE: 31.0 (on a small sample dataset).
    
5. Evaluation Results
   
The Random Forest model demonstrated superior performance compared to Linear Regression due to its ability to handle non-linear relationships and variance better. Performance metrics like MAE were calculated using test data after splitting.

6. Future Work
   
>Feature Engineering: Explore more robust feature extraction.
>Hyperparameter Tuning: Optimize model performance.
>Scaling Up: Evaluate on a larger, clean dataset.
