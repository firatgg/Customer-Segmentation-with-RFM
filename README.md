# Customer Segmentation with RFM

## Business Problem

FLO wants to segment its customers and determine marketing strategies based on these segments. For this purpose, customer behaviors will be defined, and groups will be created based on clustering these behavior patterns.

## Data

https://www.kaggle.com/datasets/busranurok/flo-data-20k/

## Dataset Story

The dataset consists of information about customers who made their last purchases in the years 2020-2021 through OmniChannel (both online and offline shopping).

- `master_id`: Unique customer number
- `order_channel`: Channel used for shopping (Android, iOS, Desktop, Mobile, Offline)
- `last_order_channel`: Channel used for the last purchase
- `first_order_date`: Date of the first purchase by the customer
- `last_order_date`: Date of the last purchase by the customer
- `last_order_date_online`: Date of the last online purchase by the customer
- `last_order_date_offline`: Date of the last offline purchase by the customer
- `order_num_total_ever_online`: Total number of purchases made by the customer online
- `order_num_total_ever_offline`: Total number of purchases made by the customer offline
- `customer_value_total_ever_offline`: Total amount spent by the customer in offline purchases
- `customer_value_total_ever_online`: Total amount spent by the customer in online purchases
- `interested_in_categories_12`: List of categories the customer has shopped in the last 12 months

## Tasks

### Task 1: Data Understanding and Preparation

1. Read the `flo_data_20K.csv` data.
2. In the dataset:
   - a. Display the first 10 observations,
   - b. Display variable names,
   - c. Display descriptive statistics,
   - d. Check for missing values,
   - e. Examine variable types.
3. Create new variables for the total number of purchases and spending for each customer, considering that omnichannel customers shop both online and offline.
4. Examine variable types and convert date-related variables to the date type.
5. Explore the distribution of the number of customers, average number of items purchased, and average spending across shopping channels.
6. List the top 10 customers with the highest revenue.
7. List the top 10 customers with the most orders.
8. Modularize the data preprocessing process.

### Task 2: Calculation of RFM Metrics

### Task 3: Calculation of RF and RFM Scores

### Task 4: Definition of RF Scores as Segments

### Task 5: Action Time!

1. Examine the averages of recency, frequency, and monetary for each segment.
2. Using RFM analysis, find customers in the relevant profiles for 2 cases and save their customer IDs to a CSV file.
   - a. FLO is introducing a new women's shoe brand. Special communication will be established with customers interested in this brand. Customers to be targeted are champions and loyal customers, with an average spending of over 250 TL in the women's category. Save the customer IDs to a CSV file named `new_brand_target_customer_ids.csv`.
   - b. A discount of approximately 40% is planned for men and children's products. Customers who were good customers in the past but haven't shopped for a long time, those who are dormant, and new customers will be targeted. Save the customer IDs to a CSV file named `discount_target_customer_ids.csv`.

### Task 6: Functionize the Entire Process
