**Marketing Campaign Data Analysis**
**Project Overview**

This project analyzes a marketing campaign dataset to understand customer behavior, purchasing patterns, and campaign effectiveness.

Using Python-based data analysis techniques, the project explores customer demographics, spending behavior, and channel preferences to generate insights that can help businesses improve their marketing strategies.

**Dataset Description**

The dataset contains customer information including:

Customer demographics
Income levels
Education
Marital status
Purchase history
Product spending
Marketing campaign responses

Key variables include:

**Feature	Description**
Income	Annual income of the customer
Age	Age calculated from birth year
Total_Spending	Total spending on all products
Total_Purchases	Total purchases across channels
Response	Whether the customer accepted the last campaign
Total_Children	Number of children at home
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
SciPy
Data Preprocessing

**The dataset required several preprocessing steps:**

• Converted Dt_Customer to datetime format
• Cleaned and converted Income column to numeric
• Handled missing values using group-based imputation
• Removed invalid categories from Marital_Status
• Created new features:

Total_Children
Age
Total_Spending
Total_Purchases

Outliers were detected and treated using the IQR method.

**Feature Engineering**

New variables were created to improve analysis:

Total_Children = Kidhome + Teenhome
Age = Current Year - Year_Birth
Total_Spending = Sum of all product spending
Total_Purchases = Web + Store + Catalog purchases

Categorical variables were encoded using:

**Ordinal Encoding → Education
One-Hot Encoding → Marital Status
Exploratory Data Analysis
**

**EDA was performed using:**

Histograms
Boxplots
Correlation heatmaps
Scatter plots
Count plots

These visualizations helped identify distribution patterns, outliers, and relationships between variables.

**Key Insights**
**1️⃣ Income Distribution**

Income shows a right-skewed distribution, indicating a large number of customers with moderate income and a smaller group of high-income customers.

**2️⃣ Spending Behavior**

Customers with higher income tend to have higher total spending, showing a strong positive correlation between income and purchasing power.

**3️⃣ Product Performance**

From the revenue analysis:

Wine products generated the highest revenue
Fruits and sweets contributed the least revenue

This suggests that premium products drive most of the sales.

**4️⃣ Customer Age & Campaign Acceptance**

The boxplot analysis shows that:
Customers who accepted the campaign tend to have slightly higher median age
However, overlapping distributions indicate a weak relationship

**5️⃣ Channel Preference**

Correlation analysis indicates:
Some relationship between web purchases and catalog purchases
Store purchases are not strongly cannibalized by other channels

**6️⃣ Children vs Spending**
Scatter plot analysis suggests:
Customers with more children tend to spend slightly less overall
This may be due to increased household expenses.

**7️⃣ Customer Complaints**

Complaint analysis shows that certain education groups lodge more complaints, which may indicate higher expectations from those customers.

**Hypothesis Testing**

A statistical test was attempted to determine whether customers in the USA make more purchases than others.

**However:**

The dataset contained very few or no USA customers
Therefore the T-test result was invalid (NaN)

This highlights a data limitation in the dataset.

**Conclusion**

This analysis provides valuable insights into customer demographics, spending behavior, and marketing campaign effectiveness.

**Key takeaways:**

Income strongly influences spending behavior
Wine products generate the highest revenue
Customers with children spend slightly less
Campaign response shows limited correlation with age

These insights can help businesses design more targeted and effective marketing strategies.

**Future Improvements**

Possible extensions for this project include:

Customer segmentation using clustering
Predictive modeling for campaign response
Customer lifetime value analysis
Marketing campaign optimization

**Author**
Nikki Malviya
Data Science & Machine Learning Enthusiast
