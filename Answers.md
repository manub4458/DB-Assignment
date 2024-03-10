Answer1.
A one-to-many link is established between the "Product_Category" and "Product" fields by the "product_category_id" field in the "Product" table. This implies that a product may be a part of multiple categories, yet a product may only be a part of one category.

Answer2.
The "product_category_id" field in the "Product" table is a foreign key referencing the primary key "id" of the "Product_Category" table. This relational constraint ensures that the value stored in the "product_category_id" field must exist as a valid category ID in the "Product_Category" table. When attempting to insert a product with an invalid category ID, the database will raise an error, thereby preventing the creation of the product.