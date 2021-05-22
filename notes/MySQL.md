# MySQL notes


### MySQL as homebrew service

```sh
brew services start mysql
brew services list
```


### reset the MySQL root password

update /etc/mysql/my.cnf and add lines:
```
[mysqld]
skip-grant-tables
```

```sh
sudo mysql mysql

mysql> UPDATE mysql.user SET authentication_string=null WHERE User='root'; FLUSH PRIVILEGES;
mysql> exit;

mysql -u root mysql;

mysql> ALTER USER 'root'@'localhost' IDENTIFIED WITH caching_sha2_password BY 'password';
mysql> exit;

brew services start mysql

mysql -u root -p
```

### stop MySQL after running it using mysqld_safe

```sh
mysqladmin shutdown
```
