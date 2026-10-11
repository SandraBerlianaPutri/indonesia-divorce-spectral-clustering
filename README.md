# Spectral Clustering of Divorce Factors in Indonesia

## About
This project applies Spectral Clustering to group Indonesian provinces based on divorce factors in 2023. The analysis identifies provincial groups with similar patterns of divorce causes.

## Data
- **Source:** [Statistics Indonesia (BPS)](https://www.bps.go.id/)
- **Period:** 2023
- **Coverage:** Provinces across Indonesia
- **Frequency:** Annual
- **Observations:** Provinces
- **Variables:** Number of divorces by seven causes, measured in people:
  - \(X_1\): Alcohol consumption
  - \(X_2\): Gambling
  - \(X_3\): Abandonment by one party
  - \(X_4\): Domestic violence (DV)
  - \(X_5\): Disputes and quarrels
  - \(X_6\): Apostasy
  - \(X_7\): Economic factors

## Methods
1. **Data Preparation** — Load the provincial dataset and separate numerical variables from province names.
2. **Exploratory Data Analysis** — Examine correlations among divorce factors using a correlation matrix and heatmap.
3. **Affinity Matrix** — Measure similarity between provinces using a Gaussian Radial Basis Function (RBF) kernel.
4. **Laplacian Construction** — Build the degree matrix and normalized symmetric graph Laplacian.
5. **Eigen Decomposition** — Extract eigenvectors associated with the smallest eigenvalues.
6. **Normalization** — Normalize eigenvector rows before clustering.
7. **Optimal Cluster Selection** — Compare silhouette scores for different cluster counts.
8. **K-Means Clustering** — Group provinces based on the normalized spectral representation.
9. **Cluster Profiling** — Summarize provincial membership and compare average divorce factors across clusters.
10. **Visualization** — Use a radar plot to compare cluster characteristics.

## Author
**Sandra Berliana Putri** - Statistics and Data Science graduate from IPB University, interested in data analysis and machine learning.
