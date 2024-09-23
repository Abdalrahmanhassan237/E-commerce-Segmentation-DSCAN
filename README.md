# E-Commerce Transaction Segmentation
![Screenshot_18-9-2024_23614_bfdogplmndidlpjfhoijckpakkdjkkil](https://github.com/user-attachments/assets/b3d3dd6d-d471-4c7c-a104-262f733315a2)

## 1. Problem Statement & Objective

### Goals
- Explore and analyze e-commerce transaction data to identify patterns and trends
- Understand customer behavior and transaction statuses across different cities and merchants

### Problems Addressed
- Lack of clarity in transaction statuses across cities and merchants
- Impact on business decisions regarding resource allocation and customer targeting

### Challenges
- Inconsistent transaction statuses
- Missing or duplicate data
- Complex relationships between merchants, cities, and transaction statuses

### Opportunity
- Identify trends in transaction statuses (e.g., cities or merchants with more burned transactions)
- Optimize business operations, enhance customer experience, and improve transaction success rates

### Importance
- Crucial for business growth, customer retention, and operational efficiency
- Significant impact on decision-making, particularly in optimizing marketing strategies and improving transaction success rates

## 2. Methodology

### Approach
1. **Exploratory Data Analysis (EDA)**
   - Visualize transaction distributions across cities and merchants.
2. **Data Cleaning**
   - Handle missing values.
   - Remove duplicates.
   - Check for outliers.
3. **Data Preprocessing**
   - Encode categorical variables.
   - Aggregate transaction data for analysis.
4. **Clustering Models**
   - Applied **K-Means** and **DBSCAN** clustering techniques to segment e-commerce transactions into meaningful groups based on transaction statuses, cities, and merchants.
   - **K-Means** clustering was performed to find the optimal number of clusters using the **Silhouette Score** and **Elbow Method**.
   - **DBSCAN** clustering was also applied to identify noise and separate dense transaction clusters.
   - The best-performing model (based on the Silhouette Score) was selected for further analysis.

### Challenges Overcome
- Handled missing values in the transaction department.
- Identified and addressed outliers during preprocessing.
- Removed unnecessary columns to streamline the dataset.
- **Clustering Challenge**: Successfully segmented the transaction data using clustering techniques to gain more insights into customer behavior and merchant performance.

## 3. Insights/Findings

### Key Findings
- Transaction status distribution (burned, subscribed) varies significantly across cities.
- Some merchants have disproportionately high numbers of burned transactions.
- Certain cities consistently have higher rates of successful transactions.
- **Cluster Analysis Findings**:
   - Clustering helped identify groups of cities and merchants where transactions either tend to succeed or fail.
   - **K-Means** clusters revealed patterns in transaction statuses across different cities, helping identify regions with better customer engagement.
   - **DBSCAN** clusters highlighted noisy and potentially problematic transactions that could be outliers or fraud-related cases.
   - 
### Visualizations
Figure 1: Stacked Bar Plot - Distribution of transaction statuses across cities

![output](https://github.com/user-attachments/assets/a925d187-2ee2-40e1-8942-8ccd75eeda9d)

Figure 2: Treemap - Transactions by merchant and status, highlighting problematic areas

![newplot](https://github.com/user-attachments/assets/310bea06-f763-4ea1-a611-4aa33539801d)

- **Figure 3**: **Elbow Method** - Optimal number of clusters based on inertia for K-Means.
- **Figure 4**: **Silhouette Score** - Evaluation of cluster quality for different K values in K-Means.

![output](https://github.com/user-attachments/assets/1fa79429-5ac7-4127-b52c-75a89d26fa25)

- **Figure 4**: **Cluster Visualization** - PCA-reduced plot of the best model clusters (K-Means or DBSCAN), showing transaction groups across cities and merchants.

![output2](https://github.com/user-attachments/assets/c2f3a9d4-3f14-497b-be70-7925b3f65809)


### Business Context
- Focus on improving merchant and city-specific operations.
- Provide targeted support for merchants with high failure rates.
- Consider expanding business efforts in high-performing regions.
- Use cluster-based insights to optimize marketing strategies and better allocate resources.


