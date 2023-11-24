# Data Cleaning

Data cleaning is an important step in the data analysis process, ensuring accuracy and credibility of insights derived from the data.

![cleaning 1](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/19b465ce-9869-4538-862a-db86e1c928b7)



## Duplicate Check

I checked for duplicates, but fortunately, no duplicates were identified.

## Churn Column

The "Churn" column has two values, 1 and 0. Here, 0 signifies an active customer, while 1 indicates a churned customer. For clarity, I created a new column called "Churned Status." Using the IF statement, I replaced 1 with "Churned" and 0 with "Active," providing a more descriptive representation of the customer status.

![Cleaning 2](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/cb33a43f-13ed-4d75-ba2d-c7c2f85a49af)


## Tenure Column

I addressed missing values by filling them with the mean value. Additionally, I created a new column named "Tenure Range" and categorized tenure into groups: 0–6 months, 1 year, 2 years, and more than 2 years for a better representation using the IF statement.

![cleaning 3](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/30e9d91a-6308-4579-8453-f7a389d92f00)

## Preferred Login Device Column

To address an inconsistency where both "Phone" and "Mobile Phone" were used to denote the same device, I used the find and replace function to replace "Mobile Phone" with "Phone" for uniformity.

![cleaning 4](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/16c31027-5346-47cb-b939-45afb7e31107)


### Steps:
Select column → CTRL+H (Find and Replace)

![cleaning 5](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/86fbf3c9-897a-454f-b74b-f04b7561811f)

## Warehouse to Home Column

I noticed missing values and addressed them by filling them with the mean of "Warehouse to Home" distances. Additionally, I observed anomalies with values 126 and 127, likely outliers or data entry errors. To rectify this issue, I used the find and replace function, adjusting the values to 26 and 27 to align them within the appropriate range for this column.

![cleaning 6](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/1a963dfb-248a-4674-bd0f-cdcf68099647)


I created a new column using the IF statement and categorized the "Warehouse to Home" distances into groups such as "Very Close Distance," "Close Distance," "Moderate Distance," and "Far Distance." This grouping provides a clearer representation of the distances.

![cleaning 7](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/3c4c3c00-f091-41e8-b371-cbd0d0be6bd1)


## Preferred Payment Mode

I noticed that "Cash on Delivery" and "COD," as well as "Credit Card" and "CC," appear in the column but mean the same thing. Using find and replace, I replaced "COD" with "Cash on Delivery" and "CC" with "Credit Card."

![cleaning 8](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/cadaffb0-760b-4ccc-b96c-b6779e1b0e50)

## Hour Spend on App Column

I noticed missing values and addressed them by filling them with the mean of the Hour spend on the app.

![cleaning 9](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/d7015dba-ea27-4296-9b8d-5d4652fdfc95)


## Preferred Order Category

"Mobile Phone" and "Mobile" represent the same thing. To maintain consistency, I replaced "Mobile Phone" with "Mobile" as the category name.

![cleaning 10](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/064b02b4-bb29-45bb-af2e-2fbbf03aa465)


## Complain Column

Here, 0 indicates customers who didn't complain, and 1 means customers who did. I created a new column called "Complaint Received" for clarity. Using the IF statement, I replaced 1 with "Yes" and 0 with "No" to provide a better representation of whether a customer has lodged a complaint or not.


![cleaning 11](https://github.com/Hagar-zakaria/Ecommerce-Churn-Analysis-Dashboard/assets/93611934/aad7054e-4353-46bf-9af3-d31f2342507b)
