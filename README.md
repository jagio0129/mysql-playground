SQL練習場
===

## Setting sample data

[MySQL TUTORIAL](https://www.mysqltutorial.org/mysql-sample-database.aspx)にあるデータ

## Database Schema

|table name|description|count|
|---|---|---|
|Customers| stores customer’s data.|122|
|Products| stores a list of scale model cars.|110|
|ProductLines| stores a list of product line categories.|7|
|Orders| stores sales orders placed by customers.|326|
|OrderDetails| stores sales order line items for each sales order.|2996|
|Payments| stores payments made by customers based on their accounts.|273|
|Employees| stores all employee information as well as the organization structure such as who reports to whom.|23|
|Offices| stores sales office data.|7|

![](https://www.mysqltutorial.org/wp-content/uploads/2009/12/MySQL-Sample-Database-Schema.png)

## Setup

```sh
# get data
#   https://www.mysqltutorial.org/mysql-sample-database.aspx
wget https://www.mysqltutorial.org/wp-content/uploads/2018/03/mysqlsampledatabase.zip
unzip mysqlsampledatabase.zip
rm mysqlsampledatabase.zip

# init
mv mysqlsampledatabase.sql docker/db/sql/
docker-compose up -d

# 確認
mycli -u root

> show databases
--------------------+
| Database           |
+--------------------+
| information_schema |
| classicmodels      |  # <= sample database
| mysql              |
| performance_schema |
| root               |
| sys                |
+--------------------+
```

## データ概要

```sql

```
