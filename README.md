# machine_learning_project-unsupervised-learning

### Project Description:
In this project, we applied unsupervised learning techniques to a real-world data set and used data visualization tools to communicate the insights gained from the analysis.

The data set for this project was the "Wholesale Data" dataset containing information about various products sold by a grocery store. The project will involved Exploratory Data Analysis and Pre-Processing, K-Means Clustering, Hierarchial Clustering and Principal Component Analysis. 

### Exploratory Data Analysis and Pre-Processing:

Initial exploration of the data shows 440 Rows of data with 8 columns. Column 3 and up appear to be numerical apparently denoting the sales of each product in "Monetary Units", with each row representing a clients of the Wholesale Distributor who is the Project Owner. Columns 1 and 2 are the Channel and Region respectively. All of the datatypes were int64. There were no missing values in the dataset. Summary statistics indicated that there might be outliers present and the The histogram shows a heavily skewed dataset not having a normal distribution.  Exploration of the boxplot also confirmed outliers far in excess of two standard deviations.  Exploration of a pairplot indicate, again, a very skewed distribution with the major linear corellation being between 'Grocery' and 'Detergents_Paper'.  The corellation matrix also confirms the highest corellation between 'Grocery' and 'Detergents_Paper' at 0.92. Although outliers were detected, the issue was that by excluding outliers we would lose information with only 440 records in the dataset so we left them in.

### K-Means Clustering

K-Means Clustering for which we picked ‘Grocery’ and ‘Detergents_Paper’ because of their correlation was inconclusive. In k-means clustering with highly skewed data, clusters may be distorted toward the majority class. This algorithm relying on means is sensitive to extreme values which this dataset has potentially leading to inaccurate results.

### Hierarchial Clustering

Hierarchial clustering showed 7 clusters, but once again in hierarchical clustering with heavily skewed data, the dendrogram may exhibit imbalanced structures emphasizing dominant clusters. Once again learning how to address skewness was the major lesson learned during this project.

### PCA Analysis

Performing a PCA analysis indicated that 4 Principal Components appeared to cover off 80% of the variance, so reducing dimensionality in this fashion would be helpful.

### Conclusions

1. In k-means clustering with highly skewed data, clusters may be distorted toward the majority class. The algorithm, relying on means, is sensitive to extreme values, potentially leading to inaccurate results.

2. In hierarchical clustering with heavily skewed data, the dendrogram may exhibit imbalanced structures, emphasizing dominant clusters.

3. PCA analysis with skewed data can be affected by outliers. Pre-processing, like log-transformations, would have helped mitigate skewness for more accurate feature identification.

4. Log Transformation should have been considered, but we ran out of time considering this entire project was only allocated 90 minutes.


