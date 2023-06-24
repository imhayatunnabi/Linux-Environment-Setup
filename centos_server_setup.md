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

## install node js and npm in server

```bash
sudo dnf module install nodejs:latest_version_number
sudo dnf module list nodejs
```

### Like node js 18 latest version

```bash
sudo dnf dnf module install nodejs:18/common
```

## php with all the necessary extensions installations

```bash
#!/bin/bash

# Install PHP and required dependencies
sudo dnf install -y epel-release
sudo dnf install -y http://rpms.remirepo.net/enterprise/remi-release-8.rpm
sudo dnf module reset php -y
sudo dnf module enable php:remi-8.2 -y
sudo dnf install -y php php-cli php-common

# Enable Remi's PHP repository
sudo dnf install -y dnf-utils
sudo dnf install -y https://rpms.remirepo.net/enterprise/remi-release-8.rpm
sudo dnf module enable php:remi-8.2 -y

# Install all available PHP extensions
sudo dnf install -y php-*
# or 
sudo dnf install -y php php-cli php-fpm php-mysqlnd php-zip php-devel php-gd php-mbstring php-curl php-xml php-pear php-bcmath php-json php-openssl php-pdo php-ldap php-pecl-imagick php-pecl-memcache php-pecl-redis php-pecl-apcu php-pecl-mongodb


# Restart Apache (if installed) or any other web server
sudo systemctl restart httpd

# Verify PHP installation
php -v

```
