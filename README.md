# K-Means Clustering Project

## Introduction
This project demonstrates the application of K-Means clustering on the "Mall Customers" dataset. It is divided into three main parts:
- Part A: Determining the optimal number of clusters using the Elbow Method.
- Part B: Applying K-Means clustering with the optimal number of clusters.
- Part C: Implementing a custom K-Means algorithm and comparing it with the standard implementation.

## Data Description
- **Mall Customers Data:** Contains customer data with attributes such as `CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, and `Spending Score (1-100)`.

## Part A: Optimal Cluster Determination
1. **Loading Data:**
    - Load the data from `Mall_Customers.csv`.
    - Extract relevant features: `Annual Income (k$)` and `Spending Score (1-100)`.

2. **Elbow Method:**
    - Apply K-Means clustering with varying numbers of clusters (k) from 1 to 10.
    - Calculate the distortion (inertia) for each k and plot the results.
    - Determine the optimal number of clusters based on the "elbow" point in the plot.

## Part B: Applying K-Means Clustering
1. **K-Means Clustering:**
    - Apply K-Means clustering with the optimal number of clusters (k=5).
    - Assign each data point to a cluster and add a `Cluster` column to the dataset.
    - Print the dataset with the assigned clusters.

2. **Centroid Calculation:**
    - Calculate and print the final centroids of the clusters.

3. **Visualization:**
    - Plot the clusters and centroids using a scatter plot.

## Part C: Custom K-Means Implementation
1. **Custom K-Means Algorithm:**
    - Implement a custom K-Means algorithm including:
        - Initializing centroids.
        - Assigning data points to clusters.
        - Updating centroids.
    - Define functions: `initialize_centroids`, `assign_data_points_to_clusters`, `update_centroids`, and `custom_kmeans`.

2. **Applying Custom K-Means:**
    - Apply the custom K-Means algorithm with the optimal number of clusters (k=5).
    - Plot the clusters and centroids using a scatter plot.

3. **Centroid Calculation:**
    - Print the final centroids of the clusters obtained from the custom K-Means algorithm.

## Dependencies
- Python 3.x
- pandas
- matplotlib
- numpy
- scikit-learn

## Usage
1. **Prepare the Environment:**
    - Ensure all dependencies are installed. You can use `pip` to install any missing packages:
      ```sh
      pip install pandas matplotlib numpy scikit-learn
      ```

2. **Run the Code:**
    - Save the provided script to a `.py` file.
    - Execute the script in your Python environment:
      ```sh
      python your_script_name.py
      ```

3. **Inspect Results:**
    - The script will generate various plots and display them.
    - The final centroids will be printed to the console.

## Results
1. **Elbow Method Plot:**
    - Displays the distortion vs. the number of clusters to determine the optimal k.

2. **K-Means Clustering:**
    - Displays the clusters and centroids for the optimal number of clusters.

3. **Custom K-Means Clustering:**
    - Displays the clusters and centroids obtained from the custom K-Means algorithm.

4. **Centroids:**
    - Final centroids of clusters printed to the console.

