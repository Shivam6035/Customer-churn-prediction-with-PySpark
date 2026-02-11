# Customer-churn-prediction-with-PySpark

# About Data

Total Records: 148 customer records are visible in the context provided.

Churn Rate: A total of 45 customers (approximately 30.4%) have 'Yes' for Churn, while 103 customers (approximately 69.6%) have 'No'.

### Demographics :

* Gender Distribution: The customers are almost equally split, with 75 Females and 73 Males.

* Senior Citizen Status: The majority of customers are not Senior Citizens (122 'No'), while 26 are Senior Citizens ('Yes').

* Partner Status: 77 customers have a Partner, and 71 do not.

* Dependents Status: 102 customers do not have Dependents, compared to 46 who do.

### Contract and Billing :

Contract Type Distribution:
* Month-to-month contracts are the most common, accounting for 87 customers.

* One year contracts have 35 customers.

* Two year contracts have 26 customers.


### Payment Method Distribution :

* Electronic check is the most frequent payment method (71 customers).

* Mailed check is used by 32 customers.

* Bank transfer (automatic) is used by 29 customers.

* Credit card (automatic) is used by 16 customers.

* Monthly Charges: The range of Monthly Charges is very wide, starting from a minimum of $18.95 to a maximum of $115.10.

* Total Charges: The values for Total Charges span from a minimum of $19.45 up to a maximum of $8129.30.

Tenure: The customer tenure ranges from 1 month up to a maximum of 72 months.

data - /content/drive/MyDrive/data for project /dataset_pyspark_churn.csv

# Customer Metrics Explained


<img width="1227" height="836" alt="image" src="https://github.com/user-attachments/assets/59a12dbe-3310-4d96-ba82-fcde2acdcf14" />

### 1. Tenure
This histogram tracks the duration of time customers have stayed with the service.

* Distribution: The data is heavily concentrated at the lower end. There is a massive spike in the first bin (0–25 units), indicating a high volume of new customers or high early-stage churn.

* Observations: After the initial spike, the frequency remains relatively steady until about 70–80 units, after which it drops off completely. Although the X-axis extends to 450, there is no visible data beyond the 100-unit mark, suggesting the majority of the customer base is relatively "young" in terms of account age.

### 2. MonthlyCharges
This chart visualizes the distribution of the monthly bills paid by customers.

* Distribution: This is a bimodal (multi-peak) distribution, showing two distinct customer segments.

* Primary Peak: There is a very sharp spike at the $20 range, likely representing customers on "Basic" or "Entry-level" plans.

* Secondary Cluster: A second, broader cluster appears between $70 and $110, indicating a large group of customers subscribed to "Premium" or bundled services (e.g., high-speed internet + TV).

### 3. TotalCharges
This histogram represents the total amount of money a customer has paid over their entire tenure.

* Distribution: The data shows a strong right skew (positive skew).

* Observations: The highest frequency is in the $0–$500 range. As the dollar amount increases, the frequency steadily decays. This aligns with the "tenure" graph; since many customers have low tenure, their total accumulated charges remain low. Only a small fraction of long-term, high-paying customers reach the $8,000+ category.


# Breakdown by Contract Type

<img width="1084" height="525" alt="newplot" src="https://github.com/user-attachments/assets/1d0e2f9a-eba6-4731-9306-0a5aaf0c40cf" />


### Month-to-month:

* This category has the highest total count of customers, nearing 4,000.

* It also exhibits the highest volume of churn (indicated in red), with approximately 1,700 customers leaving.

* The churn rate for this segment is significantly higher than any other group.

### One year:

* The total volume is much lower, around 1,500 customers.

* Retention is notably better here; the vast majority (roughly 1,300) did not churn.

* Only a small portion, approximately 200 customers, left the service.

### Two year:

* This segment has a total count of about 1,700 customers.

* It boasts the highest retention rate, with nearly all customers (about 1,650) remaining with the service.

* Churn is almost negligible in this category, represented by a very thin red sliver at the top of the bar.



