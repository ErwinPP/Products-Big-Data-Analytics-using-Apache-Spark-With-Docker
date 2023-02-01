# Products-Big-Data-Analytics-With-Apache-Spark using Docker

## Abstract
The objective of this project is to analyse various datasets in PySpark about commercial
products and rating of e-commerce website NewChic.com.<br>

## Overview of the datasets:
For this project there are three csv files one for each product
1. Shoe products 
2. Jewelry products
3. Accessories <br>

#### Features
- Category (men, accessory, jewelry, etc)
- Subcategory type of catgeory
- name of the product
- current price : price listed on the website
- raw price : total price of the product before any discounts(i.e original price of the product)
- discounts
- Currency (currency of which the price listed in)
- likes count : popularity of the product
- isnew : tells whether the product is used or not (Binary value true or false)

## Tasks:
- ### Task 1 : Extract Data<br>
        
    1. Import the necessary packages and start your spark session
    2. load the 3 datasets into 1 dataframe.
    3. Print the schema
    
<br>

- ### Task 2 : Data Transformation

    Building more features to help analyse each product For these tasks I will be
    create more columns to help get a better understanding of each product.
    First create functions which would take the dataframe as its input and return a new dataframe containing the following columns:
    1. Average price of each category
    2. Average price of each subcategory
    3. Average discount of each category 
    4. Average discount of each subcategory 
    5. Average likes of each category
    6. Average likes of each subcategory
    7. Rank of the likes of each subcategory
    8. Dense rank of the likes of each subcategory
    9. Rank of the likes of each category
    10. Dense rank of the likes of each category
    11. Rank of the discount of each category
    12. Dense rank of the discounts of each category
    13. Sum of the unused products in each category
    14. Sum of the unused products in subcategory.
    
  Call the functions i created to create the new columns and Print the schema of the dataframe to check column created.
    
<br>

- ### Task 3- Analysis

    Utilising the newly created features to answer some questions. For this task, use the
    dataframe API to answer the following questions.<br>
    
    1. Which type of product is the least popular with the users? (tip - find the feature which
       demonstrates the popularity of a product)
    2. Which type of product is the most popular with the users?
    3. Which subcategory product is the most popular with the users?
    4. Which subcategory product is the least popular with the users?
    5. In the accessory products, which subcategory was the most expensive?
    6. Which type of product had the highest discount offerings?
    7. Which type of product had the lowest discount offerings ?
    8. In the shoe's products, which subcategory was the most common?
    9. Which type of product had the most unused products listed for sale?
    10. Which subcategory product had the most unused products listed for sale?
    
<br>
    
- ### Task 4- Load Data to postgres database<br>
    1. create a new database
    2. subsequently mount a new folder.
    3. Load your dataframes as 3 different tables in the database.
