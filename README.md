# Price Calculator

__Working Steps:__
* Research MVC
* Review PHP OOP
* Import the SQL file to the Data Base
* Establish connection with the Data Base
* Create the Customer, Group & Product Classes
* Create the Customer Loader, Group Loader & Product Loader
* Connect Customer to Groups and calculate the different prices
* Create the home page, and display required data

## Learning objectives
- Apply basic OOP principles
- Import data with a database
- Learn to use an MVC

## The Mission
Today you are going to combine your new awesome OOP powers with a database.
To give you some time to get familiar with a database, this exercise only requires read access, not write access.

Make a price calculator with the following entities:
- Customer (Firstname, Lastname)
- A customer group (Name)
- A product (product name, price in cents)

A customer belongs to a customer group, which can also belong to another group (infinite).
You don't need to worry for infinite loops in this exercise.

Both a customer and a group can have a discount, which can be a percentage or a fixed amount. 

#### To calculate the price:
- For the customer group: In case of variable discounts look for highest discount of all the groups the user has.
- If some groups have fixed discounts, count them all up.
- Look which discount (fixed or variable) will give the customer the most value.
- Now look at the discount of the customer.
- In case both customer and customer group have a percentage, take the largest percentage.
- First subtract fixed amounts, then percentages!
- A price can never be negative.

