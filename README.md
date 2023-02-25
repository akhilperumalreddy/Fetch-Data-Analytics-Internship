# Fetch-Data-Analytics-Internship

## 1. Review CSV data and diagram a new structured relational data model

The dataset consists of four tables. The first table, "Users", contains information about the users who have signed up for a rewards program, such as their date of birth, gender, and location. The second table, "Brands", contains information about the brands associated with the products that users purchase, such as their category, name, and related brands. The third table, "Receipts", contains information about the receipts associated with users' purchases, including the store name, purchase date, total spent, and receipt status. Each receipt in this table is associated with a user in the "Users" table through a unique identifier. The fourth table, "Receipt Items", contains information about the items associated with each receipt, including their description, brand, and quantity purchased.

Please find below the relational data model from the above data:
![ER](https://user-images.githubusercontent.com/117230607/221326052-cfb89efa-9aa0-49a8-a314-2a7999b2b6a8.png)

Notes on the data model:
1. I have shown only the important attributes of each relational table.
2. PK: Primary Key for that table
3. FK: Foreign Key(which is primary key for some other table)


### Data Cleaning

I have performed data cleaning on the dataset using the following standard techniques:
1. Removal of null rows and columns.
2. Dropping of columns that are not deemed important.
3. Removal of leading/trailing whitespace.

You can find the code for these data cleaning techniques in the clean.ipynb notebook.


## Generate a query that answers a predetermined business question(s)

