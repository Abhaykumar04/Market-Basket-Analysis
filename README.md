## Market Basket Analysis: Understanding Customer Behavior through Association Rules Mining

### I. Introduction

1. **What is Market Basket Analysis?**
   
   Market Basket Analysis uncovers associations between items by identifying combinations of products that frequently occur together in transactions.

2. **Major Types of Market Basket Analysis**

   - **Association Rule Mining:** Identifies frequent item sets and generates rules expressing the likelihood of one item being purchased with another.
   - **Sequence Analysis:** Finds frequent item sequences and generates sequential rules describing the likelihood of one sequence being followed by another.
   - **Cluster Analysis:** Groups similar items based on attributes to identify customer segments with similar purchasing behaviors.

3. **Objective of Market Basket Analysis**

   Understand customer behavior and preferences by identifying products often purchased together. This information can be used for product recommendations, store layout optimization, and targeted marketing campaigns.

### II. Business Questions

   - Discover significant trends and patterns in customer shopping habits.
   - Answer the primary question: "Which items are frequently bought together by customers?"
   - Suggest promotions and cross-selling strategies based on identified associations.

### III. About the Dataset

   - Dataset: "The Bakery Basket" from Kaggle.
   - 20,507 entries, 4 columns, covering 9,000+ transactions from 2016-01-11 to 2017-12-03.

### IV. About this Project

   - **Algorithm:** Utilizing the Apriori Algorithm for Association Rule Mining.
   - **Metrics:**
     - Support: Frequency of item set appearance.
     - Confidence: Percentage of times item B is purchased given A was purchased.
     - Lift: Measures how much more A and B appear together compared to chance.

   - **Minimum Thresholds:**
     - Support: 1% of total transactions.
     - Lift: 1.2 (20% more often than random).

   - **Project Layout:**
     1. Install the environment
     2. Import and clean the dataset
     3. Conduct EDA and Visualizations
     4. Apply Apriori Algorithm for Market Basket Analysis

### V. Data Exploration and Visualizations

   1. **Top 20 Best Selling Items**
      ![Best Selling Items](link_to_image1)

   2. **Number of Items per Transaction**
      ![Items per Transaction](link_to_image2)

   3. **Quantity Sold by Month, Day of Week, and Hours of Day**
      ![Quantity Sold by Month](link_to_image3)
      ![Quantity Sold by Day of Week](link_to_image4)
      ![Quantity Sold by Hours of Day](link_to_image5)

### VI. Market Basket Analysis

   1. **Association Rules Results**
      ![Association Rules](link_to_image6)

   2. **Parallel Coordinates Plot, Itemsets Lift, and Itemsets Confidence**
      ![Parallel Coordinates Plot](link_to_image7)
      ![Itemsets Lift](link_to_image8)
      ![Itemsets Confidence](link_to_image9)

### VII. Insights

#### Data Exploration

   - **Best Selling Items:**
     Coffee is the most popular item, accounting for 26.7% of total sales.
   
   - **Number of Items per Transaction:**
     Over 38% of transactions consist of only one item.

   - **Sales Trends and Patterns:**
     - Monthly sales show exceptional highs from Nov 2016 to Mar 2017.
     - More items sold on weekends, especially Saturdays.
     - Peak hours for orders are from 9 AM to 2 PM.

#### Market Basket Analysis

   - 15 association rules found with min_support=0.01 and min_lift=1.2.
   - Coffee appears in 47.8% of total orders.
   - Strong associations found between {coffee, tea -> cake} and {hot chocolate -> cake}.

### VIII. Recommendations

   1. Suspend sales of low-selling items to save storage costs.
   2. Allocate resources during peak hours and offer promotions for orders after 6 PM.
   3. Introduce weekday promotions to boost sales, especially on Wednesdays.
   4. Combine items strategically based on costs, profit margins, and customer preferences.
   5. Create combos with high confidence and not-too-low support levels.

### IX. Future Analysis

   Investigate exceptional high transactions from Nov 2016 to Mar 2017, considering marketing campaigns and overall performance. Optimize conditions for improved overall performance.
