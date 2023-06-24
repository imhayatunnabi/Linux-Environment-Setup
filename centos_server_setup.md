# Centos server setup with LAMP stack

## Install apache in server

```bash
sudo dnf install httpd
sudo systemctl start httpd
sudo systemctl status httpd
```

## Check apache availability

```bash
http://your_server_ip
```

## Install mariaDB in server

```bash
sudo dnf install mariadb-server
sudo systemctl start mariadb
sudo mysql_secure_installation
```

```bash
sudo mysql
```

## Setup database and credentials

```bash
CREATE DATABASE example_database;
GRANT ALL ON example_database.* TO 'example_user'@'localhost' IDENTIFIED BY 'password' WITH GRANT OPTION;
FLUSH PRIVILEGES;
```

## Login to database

```bash
mysql -u example_user -p
```

## Install php in server

```bash
sudo dnf install php php-mysqlnd
```

## Restart apache server

```bash
sudo systemctl restart httpd
```

## Test php with apache

```bash
sudo chown -R username.username /var/www/html/
```

## Install nano or vim

```bash
sudo dnf install nano
```


