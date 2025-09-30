# Elevate Labs AI/ML Internship - Task 6: K-Means Clustering

## 📝 Objective

This repository contains the solution for **Task 6: K-Means Clustering** of the Elevate Labs AI & ML Internship. The project demonstrates the implementation of the K-Means algorithm, an unsupervised learning technique, to group the Iris flowers into distinct clusters based on their physical measurements.

---

## 🌸 Dataset

The project uses the classic **Iris Dataset** (`Iris.csv`), which contains measurements for three different species of Iris flowers. The goal is to see if the algorithm can discover these species on its own.

---

## 🛠️ Workflow & Methodology

The project follows a standard workflow for unsupervised clustering:

* **1. Data Preprocessing**: The dataset was loaded, and the non-essential 'Id' column was dropped. The features were then scaled using `StandardScaler`. This step is crucial for distance-based algorithms like K-Means to ensure all features are weighted equally.

* **2. Finding Optimal 'k' with the Elbow Method**: The Elbow Method was used to determine the optimal number of clusters ('k') for the dataset. By plotting the model's inertia (within-cluster sum of squares) for a range of 'k' values, the optimal number of clusters was identified as **k=3**.

* **3. Model Training**: A `KMeans` model from Scikit-learn was trained on the scaled data with the chosen `n_clusters=3`.

* **4. Cluster Visualization**: The resulting clusters were visualized using a scatter plot to show the distinct groupings of the data points along with their calculated centroids.

* **5. Interpretation**: The model's performance was interpreted by comparing the machine-generated cluster labels with the actual `Species` labels from the original dataset using a contingency table.

---

## 📈 Results & Interpretation

* The Elbow Method clearly indicated that **3 clusters** is the optimal number for this dataset.
* The visualization showed three well-separated clusters, confirming the inherent grouping in the data.
* The final contingency table revealed a very high alignment between the model's clusters and the actual flower species, demonstrating that the unsupervised algorithm successfully discovered the natural structure of the data.

---

## 💻 Tools and Libraries Used

* Python
* Pandas
* Scikit-learn
* Matplotlib & Seaborn

---

## 🚀 How to Run

1.  Clone this repository to your local machine.
2.  Ensure you have Python and the required libraries installed.
3.  Open and run the Jupyter Notebook (`.ipynb`) or Python script to see the complete implementation and results.
