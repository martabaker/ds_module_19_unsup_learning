# ds_module_19_unsup_learning
Unsupervised Learning Homework

## Libraries/Languages
1. Pandas
2. HoloViz (hvplots)
3. Scikit Learn
4. KMeans
5. Silhouette Score
6. Calinski-Harabasz Score
7. Standard Scaler
8. PCA

## Work Description
1. Read in a CSV of market data for a selection of cryptocurrencies using Pandas
2. Normalized the data with StandardScaler because there were some fairly significant differences between min, max, and mean for a number of the features
3. Did a PCA on the scaled data with n_clusters set to the length of the number of features in the scaled dataframe and with n_clusters set to 3. 3 principal components explained 89.5% of the variance, so more components likely could have been included. Given that there were only 7 features, PCA likely wasn't necessary, but it did improve legibility of the elbow curve and clusters a little.
4. Found the optimal k-value using KMeans, Silhouette Score, and the Calinski-Harabasz Score with both the original scaled data and the PCA data. 
5. Using the k-value, both the original scaled data and PCA data were clustered and a scatter plot was created using the 1st 2 features.
6. Both the elbow curves and scatter plots were compared using hvplots Composite Plots.

## Sources
1. https://holoviz.org/tutorial/Composing_Plots.html