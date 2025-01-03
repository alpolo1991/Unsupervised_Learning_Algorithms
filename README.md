# Unsupervised Learning Algorithms: K-means & Hierarchical Clustering

Welcome to the **Unsupervised Learning Algorithms Repository**, where we explore and implement clustering techniques such as **K-means** and **Hierarchical Clustering** to analyze and segment datasets effectively.

## Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python/data)
- [Algorithms Implemented](#algorithms-implemented)
  - [K-means Clustering](#k-means-clustering)
  - [Hierarchical Clustering](#hierarchical-clustering)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

This repository demonstrates the implementation of **unsupervised machine learning algorithms** for clustering. It uses a dataset that contains customer information, such as age, gender, annual income, and spending score, to segment customers into distinct groups. These insights can assist in creating targeted marketing strategies and understanding customer behaviors.

---

## Key Features
- **Step-by-step implementation** of K-means and Hierarchical Clustering algorithms.
- **Exploratory Data Analysis (EDA)** to visualize relationships, detect outliers, and prepare data.
- **Preprocessing pipelines** to handle missing values, scale features, and encode categorical data.
- **Model evaluation metrics** like the Silhouette Score and Calinski-Harabasz Index.
- **Visualizations** to display clustering results and dendrograms for hierarchical methods.
- Fully documented code for reproducibility and learning purposes.

---

## Dataset

The dataset used in this project is based on customer information collected from a supermarket chain. It includes:
- **CustomerID**: Unique identifier for each customer.
- **Gender**: Male or Female.
- **Age**: Customer's age in years.
- **Annual Income (k$)**: Estimated annual income in thousands of dollars.
- **Spending Score (1-100)**: Assigned score based on purchase behavior.

### Sample Data
| CustomerID | Gender | Age | Annual Income (k$) | Spending Score (1-100) |
|------------|--------|-----|--------------------|-------------------------|
| 1          | Male   | 19  | 15                 | 39                      |
| 2          | Female | 21  | 15                 | 81                      |
| ...        | ...    | ... | ...                | ...                     |

The dataset is available in the repository under the `data/` folder or [Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python/data)

---

## Algorithms Implemented

### K-means Clustering
- Groups customers into `k` clusters by minimizing intra-cluster variance.
- **Key Steps:**
  1. Determining the optimal number of clusters using the elbow method.
  2. Training the model with preprocessed data.
  3. Visualizing clusters in 2D or 3D space.

### Hierarchical Clustering
- Builds a hierarchy of clusters using either agglomerative or divisive approaches.
- **Key Steps:**
  1. Generating a dendrogram to visualize the clustering process.
  2. Cutting the dendrogram to form `k` clusters.
  3. Comparing results with K-means clustering.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/alpolo1991/unsupervised-learning-algorithms.git
  ```
2. Navigate to the project folder:
  ```shell
  cd unsupervised-learning-algorithms
  ```
3. Install the required Python packages:
  ```shell
  pip install -r requirements.txt
  ```

## Usage

1. Prepare your environment:

  - Ensure you have Python 3.8+ installed.
  - Install dependencies as described above.
    
2. Run the notebook for K-means:
```bash
jupyter notebook notebooks/k_means.ipynb
```
3. Run the notebook for Hierarchical Clustering:
```bash
jupyter notebook notebooks/hierarchical_clustering.ipynb
```

## Results

### K-means Clustering
  - Optimal number of clusters: 5 (determined using the elbow method).
  - Example visualization:

### Hierarchical Clustering
  - Example dendrogram:

## Contributing

We welcome contributions! If you'd like to contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
