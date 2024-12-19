# K-Means Clustering with Iris Dataset

## Project Overview
This project demonstrates the use of **K-Means Clustering** to perform unsupervised learning on the famous **Iris Dataset**. K-Means is a popular clustering algorithm that groups data points into clusters based on their features. The Iris dataset contains measurements for different species of flowers, making it an ideal choice to explore clustering techniques.

---

## Dataset Description
The Iris dataset contains 150 samples of iris flowers from three different species:
1. **Setosa**
2. **Versicolor**
3. **Virginica**

Each sample includes the following features:
- **Sepal Length (cm)**
- **Sepal Width (cm)**
- **Petal Length (cm)**
- **Petal Width (cm)**

The goal of this project is to cluster the data points into groups based on their similarities.

---

## Project Workflow

### 1. Loading the Dataset
- The dataset is loaded from the `sklearn.datasets` module.
- The data is converted into a pandas DataFrame for easier manipulation and visualization.

### 2. Exploratory Data Analysis (EDA)
- Summary statistics are computed to understand the data.
- Pair plots are generated to visualize relationships between features.
- Box plots and histograms are used to identify data distributions and potential outliers.

### 3. Data Preprocessing
- The dataset is scaled using **Min-Max Scaling** to normalize the feature values.

### 4. Applying PCA (Principal Component Analysis)
- PCA reduces the data to 2 dimensions for better visualization of clusters.

### 5. K-Means Clustering
- The **Elbow Method** is used to determine the optimal number of clusters by plotting the Within-Cluster-Sum-of-Squares (WCSS).
- K-Means is applied to the dataset with the chosen number of clusters.
- The **Silhouette Score** is calculated to evaluate the quality of clustering.

### 6. Visualization
- A 2D scatter plot is created to visualize the clusters.
- Silhouette plots are generated to analyze the distribution of silhouette coefficients.

---

## Installation and Setup
### Prerequisites
Ensure you have Python installed along with the following libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn`

### Installation
Install the required libraries using pip:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## How to Run the Code
1. Clone the repository

2. Run the Python script:
   ```bash
   python main.py
   ```

---

## Results and Findings
### Clustering Performance
- The Iris dataset was effectively clustered into 3 groups corresponding to the 3 species of flowers.
- **Silhouette Score**: ~0.55, indicating moderately well-separated clusters.

### Visualizations
- The 2D scatter plot shows distinct clusters for Setosa, Versicolor, and Virginica.
- The Silhouette plot validates the choice of the number of clusters.

---

## Limitations
- The K-Means algorithm assumes clusters to be spherical, which may not always be the case.
- The results depend on the initialization of centroids, which may vary across runs.

---

## Future Enhancements
- Explore other clustering algorithms like **DBSCAN** or **Hierarchical Clustering**.
- Perform clustering on other datasets to test the robustness of the pipeline.
- Enhance the visualization by adding interactive plots using tools like **Plotly**.

---

## References
- [Scikit-learn Documentation](https://scikit-learn.org/stable/modules/clustering.html)
- [Iris Dataset Overview](https://en.wikipedia.org/wiki/Iris_flower_data_set)

---

## License
This project is licensed under the MIT License - see the LICENSE file for details.
