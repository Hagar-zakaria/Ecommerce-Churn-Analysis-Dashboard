# Data Cleaning

Data cleaning is an important step in the data analysis process, ensuring accuracy and credibility of insights derived from the data.
![Cleaning Image 1](Data-Cleaning-images/cleaning1.png)


## Duplicate Check

I checked for duplicates, but fortunately, no duplicates were identified.

## Churn Column

The "Churn" column has two values, 1 and 0. Here, 0 signifies an active customer, while 1 indicates a churned customer. For clarity, I created a new column called "Churned Status." Using the IF statement, I replaced 1 with "Churned" and 0 with "Active," providing a more descriptive representation of the customer status.
![Cleaning Image 2](Data-Cleaning-images/cleaning2.png)

## Tenure Column

I addressed missing values by filling them with the mean value. Additionally, I created a new column named "Tenure Range" and categorized tenure into groups: 0–6 months, 1 year, 2 years, and more than 2 years for a better representation using the IF statement.
![Cleaning Image 3](Data-Cleaning-images/cleaning3.png)

## Preferred Login Device Column

To address an inconsistency where both "Phone" and "Mobile Phone" were used to denote the same device, I used the find and replace function to replace "Mobile Phone" with "Phone" for uniformity.
![Cleaning Image 4](Data-Cleaning-images/cleaning4.png)

### Steps:
Select column → CTRL+H (Find and Replace)
![Cleaning Image 5](Data-Cleaning-images/cleaning5.png)

## Warehouse to Home Column

I noticed missing values and addressed them by filling them with the mean of "Warehouse to Home" distances. Additionally, I observed anomalies with values 126 and 127, likely outliers or data entry errors. To rectify this issue, I used the find and replace function, adjusting the values to 26 and 27 to align them within the appropriate range for this column.
![Cleaning Image 6](Data-Cleaning-images/cleaning6.png)

I created a new column using the IF statement and categorized the "Warehouse to Home" distances into groups such as "Very Close Distance," "Close Distance," "Moderate Distance," and "Far Distance." This grouping provides a clearer representation of the distances.
![Cleaning Image 7](Data-Cleaning-images/cleaning7.png)

## Preferred Payment Mode

I noticed that "Cash on Delivery" and "COD," as well as "Credit Card" and "CC," appear in the column but mean the same thing. Using find and replace, I replaced "COD" with "Cash on Delivery" and "CC" with "Credit Card."
![Cleaning Image 8](Data-Cleaning-images/cleaning8.png)

## Hour Spend on App Column

I noticed missing values and addressed them by filling them with the mean of the Hour spend on the app.
![Cleaning Image 9](Data-Cleaning-images/cleaning9.png)

## Preferred Order Category

"Mobile Phone" and "Mobile" represent the same thing. To maintain consistency, I replaced "Mobile Phone" with "Mobile" as the category name.
![Cleaning Image 10](Data-Cleaning-images/cleaning10.png)

## Complain Column

Here, 0 indicates customers who didn't complain, and 1 means customers who did. I created a new column called "Complaint Received" for clarity. Using the IF statement, I replaced 1 with "Yes" and 0 with "No" to provide a better representation of whether a customer has lodged a complaint or not.
![Cleaning Image 11](Data-Cleaning-images/cleaning11.png)
