# Titanic Data Cleaning (Task 1)

This project cleans the Titanic dataset (`Titanic-Dataset.csv`) using the steps outlined in the Jupyter Notebook `Task1.ipynb`.

## Goal

Prepare the Titanic data for analysis by cleaning and preprocessing it.

## Steps Taken

1.  **Load & Look:** Loaded the data using `pandas` and checked basic info (shape, data types, missing values).
2.  **Fill Missing Values:**
    *   Filled missing `Age` with the median age.
    *   Filled missing `Embarked` with the most common port.
    *   Removed the `Cabin` column (too many missing).
3.  **Make Numerical:** Changed categorical columns (`Sex`, `Embarked`, `Pclass`, etc.) into numbers using one-hot encoding.
4.  **Scale Numbers:** Scaled `Age` and `Fare` columns to be between 0 and 1 (normalization).
5.  **Handle Outliers:**
    *   Used boxplots to see outliers in `Age` and `Fare`.
    *   Removed rows with outlier values in these columns using the IQR method.

## Files

*   `Task1.ipynb`: The Jupyter Notebook with all the code.
*   `Titanic-Dataset.csv`: The original dataset.
*   `README.md`: This file.

## Libraries Used

*   pandas
*   numpy
*   matplotlib
*   seaborn
*   scikit-learn (for `MinMaxScaler`)

## How to Run

1.  Install the libraries: `pip install pandas numpy matplotlib seaborn scikit-learn jupyter`
2.  Place `Titanic-Dataset.csv` in the same folder.
3.  Run `jupyter notebook` or `jupyter lab`.
4.  Open `Task1.ipynb` and run the cells.

## Outcome

The notebook produces a cleaned DataFrame ready for analysis, with no missing values (in processed columns), numerical features, scaled data, and fewer outliers in 'Age' and 'Fare'.
