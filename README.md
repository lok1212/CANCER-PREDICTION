# CANCER-PREDICTION
# t Cancer Classification Project

This project aims to classify breast cancer tumors as Malignant (M) or Benign (B) using the Breast Cancer Wisconsin (Diagnostic) Dataset.

## Dataset
The dataset contains 569 instances with 32 identifiers and features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass.
- **Target Column**: `diagnosis` (M = Malignant, B = Benign)
- **Features**: Radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension.

## Project Workflow
1. **Data Preprocessing**:
   - Handled missing values (none found).
   - Encoded the target variable: `M` to 1 and `B` to 0.
   - Feature selection: Initial models were built using `fractal_dimension_mean`.
2. **Exploratory Data Analysis (EDA)**:
   - Performed descriptive statistics and checked data info.
   - Attempted correlation analysis.
3. **Model Development**:
   - **K-Nearest Neighbors (KNN)**: Optimized using cross-validation for various K values.
   - **Logistic Regression**: Implemented as a baseline classification model.
4. **Evaluation**:
   - Models were evaluated using accuracy scores on a 20% test split.

## How to Run
1. Ensure you have `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn` installed.
2. Place `Cancer_Data.csv` in the root directory.
3. Run the Jupyter/Colab notebook cells sequentially.
