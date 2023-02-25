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


## 2. Generate a query that answers a predetermined business question(s)

Queries for all the below questions are in queries.ipynb
### 1. Which brand saw the most dollars spent in the month of June?

 ![image](https://user-images.githubusercontent.com/117230607/221328666-c3511211-3226-4c27-b469-56f4a825a0b2.png)

Kirkland signatures saw the most dollars spent in June

### 2. Which user spent the most money in the month of August?

![image](https://user-images.githubusercontent.com/117230607/221328887-ec258b96-51f1-49ad-8eca-eb616f3b7580.png)

### 3. What user bought the most expensive item?

![image](https://user-images.githubusercontent.com/117230607/221328986-550e7641-a5b4-44bf-8d53-52782f8dcfe7.png)

### 4. What is the name of the most expensive item purchased?

![image](https://user-images.githubusercontent.com/117230607/221329019-f0940c89-914a-4381-9e90-92d373d4c52e.png)

Startbucks is the most expensive item purchased

### 5. How many users scanned in each month?

![image](https://user-images.githubusercontent.com/117230607/221329058-e2956a8a-b412-4822-857a-fc0e44458e0e.png)


## 3. Choose something noteworthy about the data and share with a non-technical stakeholder

### Data Quality

Following are some noteworthy points on the quality of the data extracted. These have to be addressed to enhance it's quality.
1. We can find data to be null for a significant portion for many attributes across all tables.
2. Most of the barcode data in recepit item is missing in brands. 
3. As shown below, we can observe that a given brand has inconsistent barcode and brand code across Brands and receipt item tables. For example, Mott's fruit snacks

![image](https://user-images.githubusercontent.com/117230607/221339266-6e897b24-b8db-4a0c-8947-74028b6048f6.png)


### Burlington August Sales


Sales of most brands like Amazon, Walmart are slightly high during the end of Year. This is expected due to the hoilday season but for retailers like Burlington we see the sales are insanely high for August and following are the possible reasons for that:
1. August is typically the time of year when students are preparing for the upcoming school year which leads to increased demand for clothing, backpacks, and other items sold by Burlington.
2. Burlington, offer end-of-season sales in August to clear out inventory and make room for new merchandise.

![image](https://user-images.githubusercontent.com/117230607/221339977-6e14123d-2857-4cba-a2d6-e09eebe22665.png)
