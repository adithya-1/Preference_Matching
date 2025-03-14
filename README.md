# Preference_Matching

The project is still under development.

## Summary

The project contains a Jupyter Notebook (.ipynb) that demonstrates the use of TF-IDF (Term Frequency-Inverse Document Frequency) for text analysis and clustering. 

Below is a summary of the key points and steps covered in the notebook:

### Importing Libraries:

The notebook imports necessary libraries such as TfidfVectorizer from sklearn.feature_extraction.text, pandas, KMeans from sklearn.cluster, and other utilities like numpy, euclidean_distances, and defaultdict.

### Loading Data:

The notebook loads a CSV file (section_3.csv) containing user IDs and text data related to user interests and project ideas. The text data from two columns is combined into a single text corpus.

### TF-IDF Vectorization:

The combined text data is transformed into a TF-IDF matrix using TfidfVectorizer. This matrix represents the importance of words in the documents relative to the entire corpus.

### Clustering with KMeans:

The TF-IDF matrix is used to perform clustering using the KMeans algorithm. The initial number of clusters is determined based on the size of the embeddings.

The notebook includes functions to handle clusters that are too large or too small, ensuring that clusters are of a manageable size.

### Cluster Quality Metrics:

The notebook calculates various cluster quality metrics such as within-cluster sum of squares, average pairwise similarity, and inter-cluster distance. These metrics help evaluate the effectiveness of the clustering.

### Visualization:

The notebook includes functions to plot the within-cluster sum of squares (WCSS), cohesion, and separation to visualize the quality of the clusters.

### Iterative Clustering:

The clustering process is iterative, with steps to re-cluster large clusters and combine small clusters until all clusters are of the desired size.

### Saving Results:

The final cluster labels are assigned to the original DataFrame, and the results are saved to a CSV file (final_tf-idf_Kmeans_clusters.csv).

### Cluster Analysis:

The notebook prints the sizes of clusters after each iteration and stops when no further changes are detected or when all clusters have exactly 4 members.

### Cluster Quality Metrics Output:

The notebook outputs the WCSS and cohesion per cluster, providing insights into the compactness and separation of the clusters.

### Visualization of WCSS and Cohesion:

The notebook includes code to plot the WCSS and cohesion for each cluster, helping to visually assess the clustering performance.

### Final Output:

The notebook concludes by saving the final clustering results and printing a message indicating the completion of the clustering process.

This notebook is a comprehensive example of using TF-IDF and KMeans clustering for text analysis, with a focus on ensuring cluster quality and visualizing the results.
