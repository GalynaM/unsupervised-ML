### Unsupervised-ML

### Project description:
### Cryptocurrency Clusters: determine whether cryptocurrencies that are on the trading market can be grouped to create a classification system for the new investment.

### Used:
* PCA model, t-SNE, k-Means, elbow curve.
* The dataset was obtained from CryptoCompare https://min-api.cryptocompare.com/data/all/coinlist.
* libraries: sklearn: StandardScaler, PCA, TSNE, KMeans; matplotlib

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
* ![image](https://github.com/user-attachments/assets/54730cd7-06b7-46b4-b43f-6f3854ff41c8)


#### Cluster Analysis with k-Means 
* An elbow plot created to identify the best number of clusters.
* ![image](https://github.com/user-attachments/assets/4f87171d-5063-4b0b-99a6-db344683ce32)
* According to Elbow curve cryptocurrencies can be clustered by 4 or 5 groups.

#### Visualize Clusters using k=5 in K-Means model
* ![image](https://github.com/user-attachments/assets/eac81cd1-b574-4fe1-8697-48cf4e357c32)
