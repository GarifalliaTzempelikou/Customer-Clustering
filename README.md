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

## 1) Data cleaning
## 2) Data Visualization

<img width="950" alt="Screenshot 2023-02-28 at 10 55 36 PM" src="https://user-images.githubusercontent.com/125039071/221977707-7f630f02-75ed-40fa-98f1-decee9b08e9c.png">

Histogram
<img width="993" alt="Screenshot 2023-02-28 at 10 47 58 PM" src="https://user-images.githubusercontent.com/125039071/221977137-b5e8b083-d17d-4813-8a1d-10f373d7cd78.png">

## 3) Data Scaling
## 4) Dimentionality reduction with Principal Component Analysis (PCA)
 
 <img width="611" alt="Screenshot 2023-02-28 at 10 58 32 PM" src="https://user-images.githubusercontent.com/125039071/221978293-d5746552-2290-48d6-a42e-d752e11d3505.png">
 
## 5) Hierarchical clustering - Scipy linkage()

<img width="1016" alt="Screenshot 2023-02-28 at 11 00 29 PM" src="https://user-images.githubusercontent.com/125039071/221978667-47777bde-3e6b-4c0a-b69d-1e3749218bd3.png">


## 6) Hierarchical clustering - Sklearn agglomerative()
## 7) K-means, optimal k with elbow method

<img width="1021" alt="Screenshot 2023-02-28 at 11 01 31 PM" src="https://user-images.githubusercontent.com/125039071/221978919-a90dac14-dd7e-4247-879d-c8d61b79f5a8.png">

### At the iterative plot above we can see the ratio of Distortion Score for different number of clusters. We choose the k = 2 because there the ratio starts to decease in a linear way (the Elbow).

## silhouette_score

<img width="1014" alt="Screenshot 2023-03-16 at 10 45 51 PM" src="https://user-images.githubusercontent.com/125039071/225748719-cc6b3a0b-a5c5-4d30-ae2a-b7a9b8bda471.png">


### Examining the elbow technique and the silhouette score we decided that the best separation of our data is in two clusters.

## 8) Plotting the clusters

<img width="636" alt="Screenshot 2023-03-16 at 10 41 20 PM" src="https://user-images.githubusercontent.com/125039071/225747858-2de5faad-9deb-4147-a78a-b22afcb78154.png">


## 9) Insights about the cluster distribution

<img width="1007" alt="Screenshot 2023-03-16 at 10 42 58 PM" src="https://user-images.githubusercontent.com/125039071/225748180-f0448331-8183-45a6-a81c-5880015fbf52.png">


## 10) Conclusion

First cluster includes customers with low income ,so , low spending who are mainly young but have a big family to take care of. As a result, their low income doesn't allow them to satisfy the needs of a big family. They prefer the deal purchases because of their economic problems.

Second cluster includes customers with high income and high spending who are round 45 years old and have 0 or 1 kid. They don't need deal purchases and they spend a lot of money to several products.


# The information above can be used in planning better marketing strategies.
