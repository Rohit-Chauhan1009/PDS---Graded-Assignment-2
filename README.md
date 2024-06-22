Domain:

○ E-commerce

Business Context:

● Customer segmentation is one of the most important marketing tools at your disposal, because it can help a business to better understand its target audience. This is because it groups customers based on common characteristics.

● Segmentation can be based on the customer’s habits and lifestyle, in particular, their buying habits. Different age groups, for example, tend to spend their money in different ways, so brands need to be aware of who exactly is buying their product.

● Segmentation also focuses more on the personality of the consumer, including their opinions, interests, reviews, and rating. Breaking down a large customer base into more manageable clusters, making it easier to identify your target audience and launch campaigns and promote the business to the most relevant people

Dataset Description:

The dataset contains measurements of clothing fit from RentTheRunway. RentTheRunWay is a unique platform that allows women to rent clothes for various occasions. The collected data is of several categories. This dataset contains self-reported fit feedback from customers as well as other side information like reviews, ratings, product categories, catalog sizes, customers’ measurements (etc.)

Attribute Information:

SL.No Attribute Description

1. user_id a unique id for the customer
2. item_id unique product id
3. weight weight measurement of customer
4. rented for purpose clothing was rented for
5. body type body type of customer
6. review_text review given by the customer
7. size the standardized size of the product
8. rating rating for the product
9. age age of the customer
10. category the category of the product
11. bust size bust measurement of customer
12. height height of the customer
13. review_date date when the review was written
14. fit fit feedback

Data Citation:

● Rishabh Misra, Mengting Wan, Julian McAuley "Decomposing Fit Semantics for Product Size Recommendation in Metric Spaces". RecSys, 2018.

● Rishabh Misra, Jigyasa Grover "Sculpting Data for ML: The first act of Machine Learning". 2021.

Project Objective:

Based on the given users and items data of an e-commerce company, segment the similar user and items into suitable clusters. Analyze the clusters and provide your insights to help the organization promote their business.


This code covers all the steps mentioned in the project description. Here's a brief explanation of each step:

1-2. We import necessary libraries and load the data, then examine its basic properties.
3-4. We check for and remove duplicates, then drop unnecessary columns.
5-7. We clean the 'weight' and 'height' columns, and group similar categories in 'rented for'.
8-9. We handle missing values and examine the statistical summary of the data.

10. We treat outliers in the 'age' column using the IQR method.
11. We visualize the distribution of 'rented for' categories.

12-13. We encode categorical variables and standardize the data.

14. We apply PCA to reduce dimensionality while retaining 95% of the variance.
15. We perform K-means clustering, including finding the optimal K using the elbow method.
16. We perform Agglomerative clustering on a sample of the data, including creating a dendrogram.
17. We conduct a basic cluster analysis by visualizing the distribution of features across clusters.
