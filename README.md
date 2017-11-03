# Intro to MySQL

## The Assignment

You are a DBA from Amazon, and now you have the task of building a new small database to control the products that [Jeff Bezos adquired from Whole Foods](http://www.businessinsider.com/amazon-deal-for-whole-foods-true-genius-hedge-fund-2017-7). Please, pay attention and create the correct database with data types, this is a key performance to keep updating the database in the future.

## Deliverables

  + a github repository named `assignment-intro-to-mysql`

## Setup Instructions

  1. Connect to MySQL Server on [45.55.135.14/phpmyadmin](45.55.135.14/phpmyadmin)
  2. Create a database and add your initial letters as suffix.

  ###### Example
  
  ```sql
  CREATE DATABASE Amazon_BG; # Bill Gates
  ```

## Exercise

  ```sql
  # 1. Create a database called **Amazon**.

  # 2. Create a `Products` table with `Barcode(8)`, `Description`, `Price` fields.

  # 3. Create a `Stock` table, with `Id_Product`, `Quantity` fields.

  # 4. Add `Cookies` with barcode `07427452`, and with a cost of `$8.50`. We have `42` in stock.

  # 5. Add `Orange Juice` with barcode `12365438`, and with a cost of `$12.44`. We have `15` in stock.

  # 6. Add `Ice Cream` with barcode `98740932`, and with a cost of `$55.98`. We have `8` in stock.

  # 7. Add `Halls` with barcode `00870021`, and with a cost of `$5.21`. We have `10` in stock.

  # 8. Add `Coke` with barcode `53791253, and with a cost of `$12.34`. We have `9` in stock.

  # 9. Show me the products with more than `10` units in stock.

  # 10. Add `15` units more to `Ice Cream`.

  # 11. Show me the products with less than `10` units in stock.

  # 12. Delete `Orange Juice` from our store.

  # 13. Show me the products ordered by `Description`.

  # 14. Show me the products ordered by `price, from `highest`.

  # 15. What are the products between `$5.00` and `$10.00`.

  # 16. What are the products between `$5.00` and `$10.00`, ordered by `highest`.

  # 17. How much products do we have?

  # 18. How much stock do we have?

  ```
