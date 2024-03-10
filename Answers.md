Q1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

ANSWER: The relationship between the "Product" and "Product_Category" entities is typically a one-to-many relationship, where one product belongs to one category, but one category can have multiple products. This relationship is established through the "category_id" foreign key in the "Product" table, which references the primary key "id" in the "Product_Category" table. Essentially, each product record in the "Product" table is associated with a specific category through this foreign key relationship.


.
.







Q2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

ANSWER: To ensure that each product in the "Product" table has a valid category assigned to it, you can enforce referential integrity using foreign key constraints. This constraint will ensure that the value in the "category_id" column of the "Product" table must exist in the primary key column "id" of the "Product_Category" table. This means that whenever a new product is inserted into the "Product" table or an existing product is updated, the corresponding category must exist in the "Product_Category" table. If a category is deleted or modified in the "Product_Category" table, appropriate actions (e.g., cascade delete or update) can be specified to maintain referential integrity.
