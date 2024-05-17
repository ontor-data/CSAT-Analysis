# Problem Statement

A leading retail company aims to enhance its understanding of customer purchasing
behaviors and market dynamics to optimize inventory management, boost sales, and
improve overall customer satisfaction. By analyzing transaction data from 2009 to
2011, the company seeks to identify key trends in product popularity, revenue
generation, and purchasing patterns across different markets to inform targeted
marketing strategies and operational decisions.

# Dataset Information

The dataset includes over 1 million transaction records from 2009 to 2011, capturing details like product,
quantity, price, customer ID, and country, enabling detailed analysis of purchasing trends.
  - Shape: (1067371, 8)
  - Columns:
  - Invoice No - Invoice number. Nominal. A 6-digit integral number uniquely assigned to each transaction. If
this code starts with the letter 'c', it indicates a cancellation.
  - Stock Code - Product (item) code. Nominal. A 5-digit integral number uniquely assigned to each distinct
product.
  - Description - Product (item) name. Nominal.
  - Quantity - The quantities of each product (item) per transaction. Numeric.
  - Invoice Date - Invoice date and time. Numeric. The day and time when a transaction was generated.
  - Unit Price - Unit price. Numeric. Product price per unit in sterling (Â£).
  - Customer ID- Customer number. Nominal. A 5-digit integral number uniquely assigned to each customer.
  - Country - Country name. Nominal. The name of the country where a customer resides.

# Data Processing & Cleaning Steps

• Merged Data: Combined transaction records from 2009-2010 and 2010-2011 into a
single dataset.
• Removed Cancellations: Excluded transactions where the InvoiceNo starts with 'C',
indicating cancellations.
• Filtered Customer IDs: Removed records with missing CustomerID to ensure data
completeness.
• Formatted Dates: Converted InvoiceDate to DateTime format for more accurate
temporal analysis.
• Extended Date Attributes: Added columns for 'date', 'month', 'week', and 'time' to
facilitate detailed temporal analysis.

