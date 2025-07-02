## McDonald's Customer Segmentation and Profiling

  This project explores customer segmentation using survey data from McDonald's. It applies clustering techniques like K-Means and Gaussian Mixture Models, combined with PCA for visualization, to identify distinct customer groups based on their preferences and behavior.



# Problem Statement:

 McDonald's wants to better understand its customers to create tailored marketing strategies. This project uses customer responses to questions about food quality (e.g., "Yummy", "Greasy", "Spicy", etc.) to segment customers into distinct groups. The goal is to find natural clusters within the data and profile each segment effectively.


# Libraries Used:

* pandas: For loading and manipulating data in tabular form (DataFrames).  
* numpy: For numerical operations and array handling.  
* matplotlib: For creating static visualizations like line plots and scatter plots.  
* seaborn: Built on matplotlib, used for more attractive and statistical visualizations.  
* scikit-learn: Provides machine learning tools:
  - PCA: Reduces data dimensions to visualize and simplify clusters.  
  - KMeans: Finds groups of similar data points (clusters).  
  - GaussianMixture, BayesianGaussianMixture: Flexible clustering using probabilistic models.  
  - LinearRegression: Predicts numeric values based on input features.  
  - LabelEncoder: Converts text labels to numbers.  
  - adjusted_rand_score, confusion_matrix: For evaluating clustering performance.  


# Steps:

1. Load the Data  
   The dataset 'mcdonalds.csv' is loaded into a DataFrame.  

2. Data Preprocessing 
   - The first 11 columns (categorical "Yes"/"No" responses) are converted to binary (1/0).
   - Basic descriptive statistics are computed.

3. Dimensionality Reduction 
   - PCA is used to reduce dimensions and visualize data.
   - A biplot shows how original variables contribute to principal components.

4. Clustering 
   - K-Means clustering is applied with different values of k.
   - Gaussian Mixture Models and Bayesian Mixture Models are used to improve flexibility.
   - Segmentation is visualized in PCA-reduced space.

5. Regression Mixtures 
   - Mixture of linear regression models is applied using Expectation-Maximization .
   - Segment-wise regression analysis is performed.

6. Profiling and Interpretation 
   - Segment profile plots and separation plots are generated.
   - Clusters are interpreted based on customer preferences.


# Output:

- Cluster Assignments: Each customer is assigned to a segment.
- PCA Visualization: Shows how customer responses vary across segments.
- Segment Profile Plots: Highlight the key preferences and traits for each group.
- Model Comparisons: Helps understand differences between KMeans and Mixture Models.
