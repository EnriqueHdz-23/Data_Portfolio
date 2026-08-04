# Principal Component Analysis (PCA) and Singular Value Decomposition (SVD) Experiments

This project explores the application of **PCA** and **SVD** for dimensionality reduction, visualization, and machine learning tasks. The focus is on understanding variance, eigenvectors, and the impact of dimensionality reduction on classification performance.

---

## Variance-Covariance Matrix Example

### Objective
Illustrate the intuition behind **PCA** by computing variance-covariance matrices, eigenvectors, and eigenvalues.  
The goal is to identify principal components that capture the maximum variability in the data.

### Libraries Used
- pandas  
- numpy  
- matplotlib  
- seaborn  
- random  
- sklearn.preprocessing.StandardScaler  
- pca  

### Dataset
Municipal dataset (`municipios.csv`) loaded with pandas.  

### Main Results
- Computed variance-covariance matrix and eigen decomposition.  
- Visualized principal components and variance explained.  
- Demonstrated orthogonality of principal components.  

---

## Data Loading and Exploration (CIFAR-10)

### Objective
Apply **SVD** and **PCA** to image data for dimensionality reduction and classification.  
The goal is to evaluate how reducing dimensions affects model performance.

### Libraries Used
- tensorflow (CIFAR-10 dataset)  
- numpy  
- matplotlib  
- sklearn (PCA, KNeighborsClassifier, train_test_split, accuracy_score)  

### Dataset
CIFAR-10 dataset imported via `tensorflow.keras.datasets.cifar10`.  
Images converted to grayscale and resized for efficient decomposition.

### Main Results
1. **SVD Decomposition**  
   - Applied SVD to grayscale images.  
   - Reconstructed images using 5, 10, 20, and 50 components.  
   - Demonstrated trade-off between reconstruction quality and dimensionality.  

2. **Principal Component Visualization**  
   - Projected images into the first two principal components.  
   - Scatter plot showed clustering by class labels.  

3. **PCA in Machine Learning**  
   - Trained KNN classifier on original images.  
   - Applied PCA to reduce dimensions to 50 components.  
   - Compared accuracy of KNN with and without PCA.  
   - Highlighted PCA’s usefulness in reducing computational cost while maintaining accuracy.  

4. **Eigenvalue and Eigenvector Calculation**  
   - Computed eigen decomposition of matrix:  
     

\[
     B = \begin{bmatrix} 2 & 4 & 4 \\ 4 & 9 & 11 \\ 4 & 11 & 19 \end{bmatrix}
     \]

  
   - Extracted eigenvalues and eigenvectors using Python.  

---

## Key Takeaways
- **PCA** identifies orthogonal directions of maximum variance, enabling dimensionality reduction while preserving information.  
- **SVD** provides a powerful tool for image compression and reconstruction.  
- Dimensionality reduction improves efficiency in machine learning tasks without significant loss of accuracy.  
- Eigen decomposition is fundamental to understanding variance and principal components in multivariate data.  
