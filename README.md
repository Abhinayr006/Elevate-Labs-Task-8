# Mall Customers Clustering with K-Means

## Overview
This project performs unsupervised learning on the Mall Customers dataset using K-Means clustering to segment customers based on their features. The goal is to identify distinct customer groups for targeted marketing strategies.

## Dataset
- **File**: `Mall_Customers.csv`
- **Source**: Loaded from the path specified in the notebook.
- **Description**: Contains 200 entries with 5 columns: `CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, and `Spending Score (1-100)`. No missing values are present.

## Requirements
- Python 3.x
- Libraries:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn

## Files
- **ElevateLabsTask_8.ipynb**: Jupyter Notebook with the clustering analysis code.
- **Mall_Customers.csv**: The dataset used for this project.
- **README.md**: This file, providing an overview of the project.

## Steps
1. **Data Loading and Preprocessing**:
   - Load the dataset using pandas.
   - Drop the `CustomerID` column as it's irrelevant for clustering.
   - Encode the `Gender` column (Male=0, Female=1).

2. **Clustering with K-Means**:
   - Apply the Elbow Method to determine the optimal number of clusters (K).
   - Fit the K-Means model with the optimal K (found as K=5).
   - Assign cluster labels to the dataset.

3. **Dimensionality Reduction (Optional)**:
   - Use PCA to reduce the dataset to 2 dimensions for visualization purposes.

4. **Visualization**:
   - Visualize the clusters using scatter plots with color-coding to differentiate clusters.

5. **Evaluation**:
   - Compute the Silhouette Score to evaluate clustering quality.
   - Silhouette Score for K=5: ~0.357.

## Usage
1. Place `Mall_Customers.csv` in the directory specified in the notebook.
2. Install the required libraries:
3. Run the `ElevateLabsTask_8.ipynb` notebook in Google Colab.

## Results
- The K-Means model with K=5 identifies distinct customer segments.
- A Silhouette Score of ~0.357 indicates moderate clustering quality, suggesting the clusters are reasonably well-separated.

## Notes
- Update the dataset path in the notebook (`/content/drive/MyDrive/Colab Notebooks/8/Mall_Customers.csv`) to match your local setup.
- The Silhouette Score suggests there may be room for improvement in clustering quality, potentially by exploring other features or clustering methods.
