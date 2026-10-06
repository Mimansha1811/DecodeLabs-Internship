# 🧹 E-Commerce Dataset — Data Cleaning & Preparation Using Excel

## 📌 Project Overview

This project focuses on **Data Cleaning and Data Preparation using Microsoft Excel**.

The project uses an E-Commerce dataset containing information about orders, customers, products, quantities, prices, shipping details, payment methods, order status, tracking numbers, coupon codes, and referral sources.

The raw dataset required several data-quality checks and cleaning steps before it could be considered reliable and ready for further analysis.

The main objective of this project was to transform the raw dataset into a **clean, consistent, structured, and analysis-ready dataset using Microsoft Excel**.

> **Raw Dataset → Data Inspection → Data Cleaning → Data Validation → Clean Dataset**

---

# 🎯 Project Objectives

The main objectives of this project were:

- Understand the structure of the raw dataset
- Inspect the available columns and records
- Identify missing values
- Identify duplicate records
- Check for inconsistent data
- Correct formatting issues
- Standardize date values
- Clean text and categorical data
- Validate numerical values
- Check quantities and prices
- Verify total price calculations
- Check Order IDs and Customer IDs
- Standardize payment methods
- Standardize order statuses
- Check coupon codes
- Check referral sources
- Validate tracking numbers
- Identify potential data-quality issues
- Perform a final quality check
- Prepare the cleaned dataset for future analysis

---

# 📂 Dataset Information

The dataset represents **E-Commerce order transactions**.

Each row represents an order/transaction and contains information about the customer, product, pricing, payment, shipping, and order details.

## Dataset Columns

| Column | Description |
|---|---|
| `OrderID` | Unique identification number for each order |
| `Date` | Date on which the order was placed |
| `CustomerID` | Unique identification number of the customer |
| `Product` | Product purchased by the customer |
| `Quantity` | Number of units purchased |
| `UnitPrice` | Price of one unit |
| `ShippingAddress` | Customer shipping address |
| `PaymentMethod` | Payment method used for the order |
| `OrderStatus` | Current status of the order |
| `TrackingNumber` | Shipment tracking number |
| `ItemsInCart` | Number of items in the customer's cart |
| `CouponCode` | Coupon or promotional code used |
| `ReferralSource` | Source through which the customer reached the business |
| `TotalPrice` | Total value of the transaction |

---

# 🔍 Data Quality Issues Checked

The raw dataset was reviewed for common data-quality problems.

The following areas were checked:

- Missing values
- Duplicate records
- Duplicate Order IDs
- Missing Customer IDs
- Incorrect or inconsistent formats
- Date inconsistencies
- Extra spaces
- Inconsistent capitalization
- Invalid quantities
- Invalid prices
- Incorrect total-price values
- Inconsistent payment methods
- Inconsistent order statuses
- Inconsistent coupon codes
- Inconsistent referral sources
- Missing tracking numbers
- Unusual numerical values

---

# 🧹 Data Cleaning Process

The entire cleaning process was performed using **Microsoft Excel**.

---

## 1. Initial Data Inspection

The raw dataset was first opened and reviewed in Microsoft Excel.

The following aspects were inspected:

- Number of rows
- Number of columns
- Column names
- Data formats
- Sample records
- Missing information
- Duplicate information
- Inconsistent values

This helped establish an understanding of the overall quality of the dataset before beginning the cleaning process.

---

## 2. Identifying Missing Values

The dataset was checked for blank or missing values across the different columns.

Excel filters and sorting options were used to identify empty cells.

Missing values were reviewed based on the importance of the respective column.

For example:

- Missing coupon codes may indicate that no coupon was used.
- Missing tracking numbers may require checking the order status.
- Missing customer or order IDs require greater attention because they are important identifiers.

---

## 3. Removing Duplicate Records

Duplicate records were identified using Excel's:

**Data → Remove Duplicates**

Duplicate records were reviewed before removal to ensure that legitimate transactions were not accidentally deleted.

This helped prevent the same transaction from appearing more than once in the cleaned dataset.

---

## 4. Checking Duplicate Order IDs

The `OrderID` column was checked for repeated order identifiers.

Duplicate Order IDs were reviewed carefully because repeated IDs may indicate:

- Duplicate records
- Multiple entries belonging to the same order
- Data-entry errors

Only records identified as unnecessary duplicates were considered for removal.

---

## 5. Date Cleaning and Standardization

The `Date` column was reviewed to ensure that dates followed a consistent format.

Excel formatting tools were used to standardize the date field.

A consistent date format makes the dataset easier to sort, filter, and use for future analysis.

---

## 6. Text Cleaning

Text fields were reviewed for:

- Extra spaces
- Unnecessary characters
- Inconsistent capitalization
- Blank values
- Formatting inconsistencies

Excel tools such as:

- Find & Replace
- Sorting
- Filtering
- Text formatting

were used to improve consistency.

---

## 7. Product Name Standardization

The `Product` column was checked to ensure that product names were consistently written.

For example, differences caused by:

- Capitalization
- Extra spaces
- Typographical inconsistencies

were reviewed and standardized where appropriate.

This prevents the same product from being treated as different products because of formatting differences.

---

## 8. Quantity Validation

The `Quantity` column was checked for:

- Blank values
- Zero values
- Negative values
- Unusually large values
- Incorrect entries

Excel filters and sorting were used to identify suspicious values.

The objective was to ensure that quantities represented valid numbers of products purchased.

---

## 9. Unit Price Validation

The `UnitPrice` column was checked for:

- Blank values
- Zero values
- Negative values
- Unusual prices
- Formatting inconsistencies

The values were reviewed to identify possible data-entry errors.

---

## 10. Total Price Validation

The `TotalPrice` column was checked against the relationship:

**Total Price = Quantity × Unit Price**

Excel formulas can be used to verify the calculation:

```excel
=Quantity*UnitPrice
