# Caravan Insurance Customer Identification

This project focuses on classifying potential customers for buying Caravan insurance. The target variable is `Caravan` (Binary Classification).

## Files

- **Dataset:**
  - `caravan.csv`

- **Python Code:**
  - Jupyter notebook: `caravan.ipynb`

## Problem Statement

The goal is to classify potential customers into two categories based on their likelihood to purchase Caravan insurance. The target variable is binary (0 or 1).

## Kaggle Dataset

The dataset contains 87 variables and 9823 observations. Refer to the Kaggle link for variable descriptions: [Caravan Insurance Customer Identification](https://www.kaggle.com/kathakaliseth/caravan-insurance-customer-identification/notebook).

## Data Analysis

- **Data Splitting:**
  - The dataset was divided into two data frames, Train and Test, using the `ORIGIN` variable. The variable was then dropped.
  - Train Shape: (5822, 86)
  - Test Shape: (4000, 86)

- **Down Sampling:**
  - Due to imbalanced classification, down sampling was applied.
  - Original Value Counts: 0 - 3762, 1 - 238
  - Downsampled Value Counts: 0 - 400, 1 - 348

- **No Missing Values**
- **Feature Selection:**
  - Applied chi-sq-Test for Categorical variables with a p-value threshold limit of 0.02.
  - Reduced dimensions from 87 to 26.

- **Model Development:**
  - Initially, the model achieved 75% accuracy.
  - After reducing the p-value of the chi-sq test to 0.02, the model achieved 100% accuracy with no False Positives (FP) and False Negatives (FN).

  Accuracy: 1.0
  Confusion Matrix: 
  ```
  [[3762 0] 
  [0 238]]
  ```

## Usage

1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```

2. Navigate to the project directory:
   ```bash
   cd Caravan-Insurance-Customer-Identification
   ```

3. Explore the dataset and Jupyter notebook for detailed analysis and code.

Feel free to refer to the `caravan.ipynb` for an in-depth explanation of the project.

---

**Note:** Adjust file paths and comments as needed for your project structure.
