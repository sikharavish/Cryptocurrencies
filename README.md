# Cryptocurrencies

# Overview

## Our client is looking to get into the Crypto Currency market.  This analysis is focused on showing them what cryptocurrencies are currently trading and how they can be grouped together to form a classification system.  Since there is no known outcome, an unsupervised machine learning model will be used to preprocess the data and group the cryptocurrencies using a clustering algorithm.  Data visualizations will be used to share the findings.

# Results

## The original data frame(shown below) needed to be cleaned in ordered to fit into our machine learning model.

![crypto_df_orig](https://user-images.githubusercontent.com/106286533/193864552-d6bc6fd2-e1b5-40b3-8b98-a9c8fc630eba.png)

## To clean the data, we filtered to only cryptocurrencies that were trading, and had a working algorithm.  Then, null values were dropped along with unnecessary columns.

![clean_crypto_df](https://user-images.githubusercontent.com/106286533/193864737-db7d2c1c-6d25-46f3-adb9-653524aceb33.png)
![crypto_names_df](https://user-images.githubusercontent.com/106286533/193864774-afea85d0-65b3-4122-b4af-9fb884db091a.png)

## After getting dummy values for string columns, a new dataframe was create using PCA that just had our 3 principal components. 

![pcs_crypto_df](https://user-images.githubusercontent.com/106286533/193864842-b105a2af-584f-46dd-ac92-0e30f1f655e2.png)

## Kmeans and an Elbow Curve was used to find the best value for the model.

![Elbow_Curve](https://user-images.githubusercontent.com/106286533/193864880-a83cf755-1daf-489f-ab74-14310e3f3c13.png)

## After getting the predicted clusters another dataframe was created to show them with the cryptocurrency features.

![clustered_df](https://user-images.githubusercontent.com/106286533/193864971-5bb450ea-2f5b-4d00-a775-0d2abda20107.png)

## A 3D scatter plot shows the PCA data and clusters.

![3D_Scatter](https://user-images.githubusercontent.com/106286533/193865028-3c58991f-a788-4f6c-bfbb-8db0b7131c8c.png)

## Tradable CryptoCurrency Table was created using hvplot.

![Tradable_Crypto_Table](https://user-images.githubusercontent.com/106286533/193865095-c6a4521f-540f-4353-b9af-aea136c3a709.png)

## Finally a scatter plot was created to show the Total Coins Mined and Total Coin Supply for each cryptocurrency.

![Plot_df_Scatter](https://user-images.githubusercontent.com/106286533/193865150-cc8f0ed2-2068-4eb5-a847-8e3d69c1a80e.png)
