# SVM Classification on the Wine Dataset

This repository demonstrates a complete workflow for multiclass classification using **Support Vector Machines (SVMs)** on the Wine dataset. It covers data loading, preprocessing, model training, evaluation, and multiple visualization techniques, ensuring both clarity and reproducibility.

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Features & Visualizations](#features--visualizations)  
3. [Prerequisites & Installation](#prerequisites--installation)  
4. [Usage](#usage)  
5. [Repository Structure](#repository-structure)  
6. [Detailed Explanation](#detailed-explanation)  
7. [Results](#results)  
8. [Accessibility](#accessibility)  
9. [License](#license)  

---

## Project Overview

The **Wine dataset** is a classic benchmark in machine learning, containing 13 chemical/physical features of wine samples from three cultivars (multiclass problem). This project uses an **SVM** with the **RBF kernel** to classify these wine samples with high accuracy. By following the included code and instructions, you will learn how to:

- Load and preprocess a multiclass dataset.  
- Train and tune an SVM for optimal performance.  
- Evaluate model metrics, including a classification report and confusion matrix.  
- Visualize results using a **PCA-based decision boundary**, a **feature correlation heatmap**, and a **PCA scatter plot**.

---

## Features & Visualizations

1. **Data Preprocessing**  
   - Standardizes all features to ensure SVM stability and improved accuracy.

2. **SVM Model Training**  
   - Employs the RBF kernel, which effectively handles non-linear class boundaries.

3. **Performance Metrics**  
   - Generates a classification report (precision, recall, F1-score) and a confusion matrix.

4. **Rich Visualizations**  
   - **Confusion Matrix** heatmap for quick insight into class-wise performance.  
   - **PCA Decision Boundary** to illustrate how the SVM separates classes in a 2D projection.  
   - **Feature Correlation Heatmap** revealing relationships among wine features.  
   - **PCA Scatter Plot** to show inherent class separability.

5. **Multiclass Setup**  
   - Demonstrates how SVM handles three distinct classes (class_0, class_1, class_2).

---

## Prerequisites & Installation

- **Python 3.7+**  
- [NumPy](https://numpy.org/)  
- [pandas](https://pandas.pydata.org/)  
- [matplotlib](https://matplotlib.org/)  
- [seaborn](https://seaborn.pydata.org/)  
- [scikit-learn](https://scikit-learn.org/stable/)  

## Detailed Explanation

### Data Loading
We retrieve the Wine dataset using `load_wine()` from `sklearn.datasets`. This includes 13 features, a target vector (three classes), and feature names.

### Preprocessing
- **StandardScaler** normalizes all features to zero mean and unit variance.
- A **train–test split** (70% training, 30% testing) ensures unbiased evaluation.

### Model Training
- An **SVM with RBF kernel** (`C=1.0, gamma='scale'`) is trained on the standardized data.
- `probability=True` is set to enable probability estimates.

### Evaluation
- A **classification report** displays precision, recall, F1-scores, and accuracy for each of the three classes.
- A **confusion matrix** is rendered as a heatmap for quick inspection of misclassifications.

### Visualization
- **Confusion Matrix:** Showcases actual vs. predicted classes in a color-coded grid.
- **PCA Decision Boundary:** Projects data into 2D via PCA and plots SVM decision contours.
- **Feature Correlation Heatmap:** Highlights linear relationships among the 13 wine features.
- **PCA Scatter Plot:** Depicts the dataset’s separability in a reduced two-dimensional space.

## Results
Typical results (exact figures may vary slightly due to random initialization):
- **Accuracy:** ~98%
- **Precision, Recall, F1:** Near-perfect values for all three classes.
- **Plots:** Minimal overlap between classes in PCA space, confirming strong separability.

## Accessibility
- **Color Schemes:** We use colorblind-friendly palettes (`YlGnBu`, `coolwarm`, `viridis`) and large font sizes.
- **Clear Labeling:** Each plot has descriptive titles, axis labels, and legends.
- **Screen Reader Compatibility:** Titles and labels are set so that screen readers can interpret the figures.
- **Transcripts/Closed Captions:** (Recommended if delivering video or audio content.)

## License
This project is distributed under the **MIT License**. You are free to use, modify, and distribute this code for personal or commercial purposes, provided you include the original license text.


## **Clone the Repository:**
 ```bash
 git clone https://github.com/siddhartha03036/multi_class_svm.git
