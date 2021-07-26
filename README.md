SQL練習場
===

### Setting sample data
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
