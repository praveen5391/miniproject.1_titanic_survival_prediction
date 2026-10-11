# Titanic Survival Prediction — Mini Project 1

## Project Overview

This mini project uses the Titanic passenger dataset to practise data inspection, missing-value handling, categorical encoding, and basic data visualization with Python. The current notebook focuses on **data cleaning and exploratory data analysis (EDA)**; it does not train or evaluate a survival-prediction model yet.

## Objectives

- Inspect the dataset's dimensions, columns, data types, and descriptive statistics.
- Identify missing values in the passenger data.
- Fill missing `Age` values with the median age.
- Replace missing `Cabin` values with `Unknown`.
- Fill missing `Embarked` values with the most frequent category (mode).
- Convert `Sex` categories into numeric labels using scikit-learn's `LabelEncoder`.
- Apply one-hot encoding to `Embarked` and add the resulting indicator columns.
- Plot the distribution of passenger ages with Matplotlib.
- Export the processed data to a CSV file.

## Tools and Libraries

- Python
- Pandas
- Matplotlib
- scikit-learn
- Google Colab / Jupyter Notebook

## Dataset

The project uses the Titanic training dataset commonly distributed as `train.csv`.

- Original dataset: **891 rows × 12 columns**
- Exported cleaned dataset: **891 rows × 15 columns**
- Missing values in the exported CSV: **0**

The processed CSV includes the original `Embarked` column plus the one-hot encoded columns `Embarked_C`, `Embarked_Q`, and `Embarked_S`.

## Data Preprocessing

| Column | Treatment |
|---|---|
| `Age` | Missing values filled with the column median |
| `Cabin` | Missing values replaced with `Unknown` |
| `Embarked` | Missing values filled with the mode; one-hot indicator columns added |
| `Sex` | Converted to numeric labels using `LabelEncoder` |

## Visualization

The notebook creates a histogram titled **“Age Distribution of Titanic passengers”** using Matplotlib. It shows how passenger ages are distributed across age ranges. Since missing ages are imputed with the median, the filled values also affect the histogram.

## Repository Files

- `miniproject1.ipynb` — notebook containing the exploration, preprocessing steps, and visualization.
- `cleaned_titanic.csv` — exported dataset after preprocessing.
- `README.md` — project documentation.

## How to Run

1. Open `miniproject1.ipynb` in Google Colab or Jupyter Notebook.
2. Upload the original `train.csv` file when prompted, or place it in the notebook's working directory.
3. Run the notebook cells in order.
4. The notebook writes `cleaned_titanic.csv` and includes a Google Colab download cell.

## Current Status and Next Steps

**Completed:** dataset inspection, missing-value treatment, categorical encoding, CSV export, and age-distribution visualization.

**Not yet implemented:** training a machine-learning model to predict `Survived`, evaluating its performance, and reporting metrics. Those steps would be the next extension if the goal is a complete survival-prediction project.

## Learning Outcomes

- Inspecting tabular data with Pandas
- Handling missing values with median and mode imputation
- Encoding categorical variables
- Creating a histogram with Matplotlib
- Exporting a processed dataset to CSV

---

**Project name:** Mini Project 1 — Titanic Survival Prediction  
**Current focus:** Data Cleaning and Exploratory Data Analysis