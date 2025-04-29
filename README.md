# Bank-Customer-Segmentation-in-Python
This project uses K-Means Clustering to segment bank customers based on key features such as number of products, balance, and geography.

## Project Objectives

### Objective 1: Prepare the Data for Modeling
- Read the `Bank_Churn.csv` file and preview the top 5 rows.
- Create a DataFrame containing all fields except `"CustomerId"`, `"Surname"`, and `"Exited"`.
- Make all text fields numeric.
- Explore the data by looking at the min/max values and the distribution of each column.
- Create a new column called `ProductsPerYear`.

---

### Objective 2: Segment the Customers Using K-Means Clustering
- Standardize the data so that each column has a mean of 0 and a standard deviation of 1.
- Fit K-Means clustering models on the standardized data with 2–15 clusters to create an inertia plot.
- Identify the elbow point of the inertia plot and fit a K-Means model using the selected value of k.
- Check the number of customers in each cluster.
- Create a heatmap of cluster centers and interpret the clusters.

---

### Objective 3: Segment the Customers Using a Different Subset of Fields
- Examine the summary statistics by country and exclude the country fields.
- Fit K-Means clustering models on the standardized data (excluding country fields) with 2–15 clusters to create an inertia plot.
- Identify the elbow point of the inertia plot and fit a K-Means model using the selected value of k.
- Check the number of customers in each cluster.
- Create a heatmap of cluster centers and interpret the clusters.

---

### Objective 4: Further Explore Clusters and Make Recommendations
- Create a DataFrame combining the dataset from Objective 1, the `"Exited"` field, and the cluster labels.
- View the churn rate (percentage of customers who "Exited") for each cluster.
- View the country breakdown for each cluster.
- Make recommendations for how to cater to each customer segment.
