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

### Examining the elbow technique and the silhouette score we decided that the best separation of our data is in three clusters.

## 8) Plotting the clusters

<img width="665" alt="Screenshot 2023-02-28 at 11 03 03 PM" src="https://user-images.githubusercontent.com/125039071/221979113-4f5d4b11-2c07-4878-823b-7bd53d6c5610.png">


## 9) Insights about the cluster distribution

<img width="1009" alt="Screenshot 2023-02-28 at 11 03 44 PM" src="https://user-images.githubusercontent.com/125039071/221979277-df547bdd-8569-43ce-8209-73a47c55bea1.png">


## 10) Conclusion

First cluster includes customers with high income and high spending who are >45 and have 0 or 1 kid. They don't need deal purchases and they spend a lot of money to several products.

Second cluster includes customers with average income and average spending. They don't seem to have economic problems but they don't live in abundance either.

Third cluster includes customers with low income ,and so, low spending who are mainly young but have a big family to take care of. As a result, their low income doesn't allow them to satisfy the needs of a big family. They prefer the deal purchases because of their economic problems.

# The information above can be used in planning better marketing strategies.
