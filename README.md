## unsupervised-ML

## Project description:
### Cryptocurrency Clusters: determine whether cryptocurrencies that are on the trading market can be grouped to create a classification system for the new investment.

### Used:
* PCA model, t-SNE, k-Means, elbow curve.
* The dataset was obtained from CryptoCompare https://min-api.cryptocompare.com/data/all/coinlist.

### Cryptocurrency Clusters.ipynb

#### Data Preparation
* Data was cleaned:
  - filtered for currencies that are currently being traded;
  - all rows that have at least one null value removed;
  - filtered for cryptocurrencies that have been mined;
* Droped non significant columns.
* Categorical variables encoded using pd.get_dummies().

#### Dimensionality Reduction
* Performed dimensionality reduction with PCA with 90% explained variance.
* Further reduced the dataset dimensions with t-SNE and result visualized.

#### Cluster Analysis with k-Means 
* An elbow plot created to identify the best number of clusters.
