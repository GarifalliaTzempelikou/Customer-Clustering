# Customer Segmentation -Clustering
The purpose of this project is to perform unsupervised clustering for customer segmentation. To achieve this we did use dimensionality reduction followed by linkage and agglomerative clustering. Additionally, we did use both visuals and statistical methods (elbow and silhouette) to identify a cluster multiplicity.

![image](https://user-images.githubusercontent.com/125039071/221970656-b117384c-1230-4ae1-9519-dcf7fa0a1cec.png)

# The dataset (Customer Personality Data)

Column description:

- ID: Customer’s unique identifier
- Year_Birth: Customer's birth year
- Education: Education Qualification of customer
- Marital_Status: Marital Status of customer
- Income: Customer's yearly household income
- Kidhome: Number of children in customer's household
- Teenhome: Number of teenagers in customer's household
- Dt_Customer: Date of customer's enrollment with the company
- Recency: Number of days since customer's last purchase
- MntWines: Amount spent on wine
- MntFruits: Amount spent on fruits
- MntMeatProducts: Amount spent on meat products
- MntFishProducts: Amount spent on fish products
- MntSweetProducts: Amount spent on sweet products
- MntGoldProds: Amount spent on gold products
- NumDealsPurchases: Number of deal purchases
- NumWebPurchases: Number of web purchases
- NumCatalogPurchases: Number of catalog purchases
- NumStorePurchases: Number of store purchases
- NumWebVisitsMonth: Number of web visits of the month
- AcceptedCmp3/AcceptedCmp4/AcceptedCmp5/AcceptedCmp1/AcceptedCmp2/Response: Promotion
- Complain
- Z_CostContact
- Z_Revenue


# The main steps

- Data cleaning
- Data Visualization

<img width="993" alt="Screenshot 2023-02-28 at 10 47 58 PM" src="https://user-images.githubusercontent.com/125039071/221977137-b5e8b083-d17d-4813-8a1d-10f373d7cd78.png">

- Data Scaling
- Dimentionality reduction with Principal Component Analysis (PCA)
- Hierarchical clustering - Scipy linkage()
- Hierarchical clustering - Sklearn agglomerative()
- K-means, optimal k with elbow method
- Plotting the clusters
- Insights about the cluster distribution
- Conclusion


