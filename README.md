# Wine Dataset Visualization & Classification

This project explores the classic [Wine dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_wine.html) from scikit-learn. 
The goal is to visualize the data, understand feature relationships, and build a simple classification model to predict wine types based on chemical attributes.

---

## Dataset Overview

- **Number of Instances:** 178  
- **Number of Features:** 13 numeric attributes + 1 target label  
- **Classes:**
  - `class_0`
  - `class_1`
  - `class_2`

---

## Features

- Alcohol  
- Malic acid  
- Ash  
- Alcalinity of ash  
- Magnesium  
- Total phenols  
- Flavanoids  
- Nonflavanoid phenols  
- Proanthocyanins  
- Color intensity  
- Hue  
- OD280/OD315 of diluted wines  
- Proline  

---

## Project Goals

- Perform exploratory data analysis (EDA)
- Visualize relationships between features and wine classes
- Train a classification model
- Evaluate model performance using precision, recall, F1 score, and confusion matrix

---

## Visualizations

### Scatter Plots (Seaborn)
- `Flavanoids vs Color Intensity`  
- `Flavanoids vs Proline`  
- `Alcohol vs Color Intensity`  
All colored by wine class (`target_name`), using `sns.scatterplot()`.

### Seaborn Pairplot
- Visualizes multiple pairwise relationships at once (e.g., Alcohol, Flavanoids, Color Intensity, Proline)
- Helps reveal feature correlations and class separation in a grid-style view

---

## Model Training

- **Model Used:** Logistic Regression/ Multiclass Classification
- **Accuracy:** 94.44% (`model.score = 0.9444`)
- **Evaluation Metrics:**  
  - **Classification Report:** Precision, Recall, F1-score  
  - **Confusion Matrix:** Visualized with `seaborn.heatmap`

---

## How to Run

1. Clone the repository or download the notebook
2. Install dependencies:
    ```bash
    pip install matplotlib seaborn scikit-learn pandas
    ```
3. Run the notebook:
    ```bash
    jupyter notebook
    ```
4. Open `wine_classification.ipynb` and execute cells

---

## Files

- `wine_classification.ipynb` — Notebook with EDA, model training, and evaluation
- `README.md` — Project overview and setup instructions

---

## Credits

- Dataset: [UCI ML Wine Dataset](https://archive.ics.uci.edu/ml/datasets/Wine)
- Tools: Python, pandas, matplotlib, seaborn, scikit-learn

