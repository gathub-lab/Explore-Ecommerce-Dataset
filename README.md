# Explore-Ecommerce-Dataset
## 1. Introduction
This is an eCommerce dataset exploration project using SQL on Google BigQuery. The dataset is based on the Google Analytics public dataset and contains data from an eCommerce website.

## 2. Requirements
* [Google Cloud Platform account](https://bit.ly/3KfVIBK)
* [Google BigQuery API](https://cloud.google.com/bigquery/docs/reference/rest) eneble
* [SQL query editor](https://cloud.google.com/monitoring/mql/query-editor) or IDE
  
## 3. Dataset access
The Ecommerce dataset is stored in the public Google BigQuery dataset. Follow these steps to access the dataset on Google Big Query:
1. Sign in to your Google Cloud Platform account and create a new project.
2. Navigate to the BigQuery dashboard and select your newly created project.
3. In the navigation panel, select "Add Data" and then select "Search Projects".
4. Enter the project ID "bigquery-public-data.google_analytics_sample.ga_sessions" and click "Enter".
5. Click on the table "ga_sessions_" to the dataset.

## 4. Exploring the Dataset
Use SQL in Google BigQuery against the Google Analytics data set to write and execute queries to find the desired data for the purpose of answering business questions

### Query 01: calculate total visit, pageview, transaction for Jan, Feb and March 2017 (order by month).
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:611d7a6be39d4da3a659047139c4f1e3)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/53463712-181a-4bc8-b80b-dbbca5500c63)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/ef59e4b2-e138-40a4-af2b-73ff987234dc)

### Query 02: Bounce rate per traffic source in July 2017 (Bounce_rate = num_bounce/total_visit) (order by total_visit DESC).
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:9c499f68b4214f6598d0219586a3eb0b)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/22b7e248-3367-41c4-843f-bf1ba6a37316)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/52beb7bc-9183-49b2-bb1f-120214ed6cbe)

### Query 03: Revenue by traffic source by week, by month in June 2017.
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:31cdc86018214f28ab302ae106a3a97a)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/d5ca46a5-763e-4c50-a78d-1f2f58004de1)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/815269f0-1512-42d1-aa66-22553e44894e)

### Query 04: Average number of pageviews by purchaser type (purchasers vs non-purchasers) in June, July 2017.
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:5ae3185342a14b1ca276c2d04284c9c5)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/192c3296-8821-4a98-b7b5-e0102434cbbd)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/cec6c180-63c2-4e3d-b0b0-9a0a8b20c152)

### Query 05: Average number of transactions per user that made a purchase in July 2017
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:14e564635f154e6d8fe8e334a08e6f50)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/60475a8e-271a-4be3-b33d-11eff0cd3c75)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/65d04280-b23e-4c77-9814-d124a2acb10d)

### Query 06: Average amount of money spent per session. Only include purchaser data in July 2017
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:858bbffbe1104c0e8964283bfefd4bb0)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/c6f1e84d-2cf7-4eef-acb6-a89f9e9e99b0)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/5e985c52-d695-4bb6-8d1d-3e20e2b8d837)

### Query 07: Other products purchased by customers who purchased product "YouTube Men's Vintage Henley" in July 2017. Output should show product name and the quantity was ordered.
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:241a2f7dd2364c46a4f26cd3c27f535a)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/e9b8a644-0729-42b5-8b26-89c7e33eb980)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/e510f31c-f301-47ba-aee6-b1738762674f)

### Query 08: Calculate cohort map from product view to addtocart to purchase in Jan, Feb and March 2017. For example, 100% product view then 40% add_to_cart and 10% purchase. Add_to_cart_rate = number product  add to cart/number product view. Purchase_rate = number product purchase/number product view. The output should be calculated in product level.
[Link to Bigquery](https://console.cloud.google.com/bigquery?sq=580650386557:37a0fb1c8afb4a6f9d1f1b150a49017f)
#### SQL code
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/242657a2-1685-4058-86ed-24c9b4b7d363)
#### Query Results
![image](https://github.com/gathub-lab/Explore-Ecommerce-Dataset/assets/116141004/dfb8a825-9a2f-4dff-892a-79ecd3340e20)

