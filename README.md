# FLD-PCA-and-Clustering-for-Image-Data
Machine Learning Techniques with FLD, PCA, and Clustering for Image Data
# Dimensionality Reduction and Unsupervised Learning

This repository contains the implementation and analysis of **dimensionality reduction** and **unsupervised learning techniques**.

## Project Objectives

1. Practice the use of **dimensionality reduction** as a preprocessing step and study its impact on classification performance.
2. Gain an in-depth understanding of **unsupervised learning algorithms** by formulating an image compression problem in this context.

---

## Project Tasks and Deliverables

### Task 1: Dimensionality Reduction

#### 1.1 Implement Fisher's Linear Discriminant (FLD)
- **Objective**: Perform supervised dimensionality reduction using class label information.
- **Deliverables**:
  - FLD module implementation.
  - Reduced dataset visualization.
  - Comparison of original and reduced images (MNIST, 3x3 reduced representation).
  
  *Include visualizations of the original and reduced MNIST images.*

#### 1.2 Implement Principal Component Analysis (PCA)
- **Objective**: Apply unsupervised dimensionality reduction to MNIST dataset.
- **Deliverables**:
  - PCA module implementation.
  - Dataset visualization after PCA (2D projections).
  - Error rate results for different dimensions (e.g., 2D, 10% error rate).

  *Graphs for PCA 2D projections should be included.*

#### 1.3 Impact of Dimensionality Reduction on Classification
- **Objective**: Analyze the effect of dimensionality reduction (FLD and PCA) on classification performance.
- **Deliverables**:
  - Classification accuracy vs. error rate plot (PCA: 5% to 30%).
  - Table comparing classifiers (Euclidean Distance, kNN, BPNN) on different datasets (nX, fX, pX).

  *Include the classification accuracy vs. error rate plot and the performance comparison table.*

### Task 2: Unsupervised Learning

#### 2.1 k-Means and Winner-Take-All (WTA) Clustering
- **Objective**: Perform image compression by clustering RGB values of a flower image.
- **Deliverables**:
  - k-Means and WTA module implementations.
  - Scatter plots of RGB space clustering results.
  - Pseudo-color images and RMSE values for k=4, 16, 64, and 256.
  - Convergence curves for both algorithms (k=16).

  *Include scatter plots, pseudo-color images, and convergence curves.*

#### 2.2 Hierarchical Clustering
- **Objective**: Solve the image compression problem using hierarchical clustering.
- **Deliverables**:
  - Results for different linkage methods.
  - Comparison with k-Means and WTA on image quality, run-time, and RMSE.

  *Include hierarchical clustering results and comparison insights.*

---

## Summary of Results

- **Dimensionality Reduction**: FLD+PCA demonstrated better class separability than PCA alone.
- **Classification Performance**: Reduced datasets (fX and pX) achieved significant computation time reductions with minimal impact on accuracy.
- **Image Compression**: k-Means offered the fastest and most consistent results, while hierarchical clustering provided better quality for larger clusters.

---

## File Structure

- `src/`: Source code for all implementations.
- `data/`: MNIST and flower image datasets.
- `notebooks/`: Jupyter Notebooks for analysis and visualization.
- `results/`: Generated graphs, tables, and reports.

---

## How to Run

1. Clone this repository.
2. Install required dependencies (listed in `requirements.txt`).
3. Run the provided Jupyter Notebooks or Python scripts in the `src/` directory for individual tasks.

---

## Example Outputs

- **Original vs. Reduced Images (MNIST)**:
  ![Example Reduced Images](path/to/reduced_images.png)

- **PCA 2D Projections**:
  ![PCA Projections](path/to/pca_projections.png)

- **Classification Accuracy vs. Error Rate**:
  ![Accuracy Plot](path/to/accuracy_plot.png)

- **k-Means Clustering Results (k=16)**:
  ![k-Means Clusters](path/to/kmeans_clusters.png)

---

## License

This project is licensed under the MIT License. See `LICENSE` for more details.

---

## References

- Maaten, L., & Hinton, G. (2008). "Visualizing data using t-SNE." *Journal of Machine Learning Research, 9*(Nov), 2579-2605.
