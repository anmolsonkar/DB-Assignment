# Database Schema Explanation

## 1. Explain the relationship between the "Product" and "Product_Category" entities.

The relationship between the "Product" and "Product_Category" entities is a one-to-many relationship. The "Product" table has a column called "category_id" which is a foreign key referencing the "id" column in the "Product_Category" table. This means that each product belongs to a single category, but a category can have multiple products associated with it.

## 2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

To ensure that each product in the "Product" table has a valid category assigned to it, you can implement a foreign key constraint on the "category_id" column in the "Product" table. This constraint would ensure that the "category_id" value for each product record must match an existing "id" value in the "Product_Category" table. Additionally, you could set the "category_id" column to "NOT NULL" to prevent products from being created without a category assigned.
