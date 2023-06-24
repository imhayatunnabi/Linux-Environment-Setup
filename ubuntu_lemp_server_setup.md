## Install wget

```
sudo apt install wget
```

## Google Chrome install

```
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```
```
sudo apt install ./google-chrome-stable_current_amd64.deb
```

## Install php storm:

## Install snap beforehand:

```
sudo apt-get install snapd
```
```
sudo snap install phpstorm --classic
```

## Install Vs code

```
sudo apt-get install wget gpg
```
```
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
```
```
sudo install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/
```
```
sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/trusted.gpg.d/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list'
```
```
rm -f packages.microsoft.gpg
```

## Then update the package cache and install the package using:

```
sudo apt update
```
```
sudo apt install apt-transport-https
```
```
sudo apt update
```
```
sudo apt install code
```

### Install git on Linux

```
sudo apt-get update
```
```
sudo apt-get install git
```
```
git config --global user.name "your github username"
git config --global user.email "your github attached email address"
```
```
ssh-keygen -t rsa -b 4096 -C "your github attached email address"
```
```
eval "$(ssh-agent -s)"
```
```
ssh-add -K /Users/you/.ssh/id_rsa
```

## Network manager:

```
sudo apt install network-manager
```
```
sudo apt update
```
```
sudo apt upgrade
```
```
sudo lshw -C network
```

## Install Nginx Server

### Ngnix:

```
sudo apt install -y php-mbstring php-xml php-fpm php-zip php-common php-fpm php-cli unzip curl nginx
```
```
sudo apt-get install nginx
```
```
sudo apt install software-properties-common
```
```
sudo add-apt-repository ppa:ondrej/php
```
```
sudo apt update && sudo apt upgrade
```
```
sudo apt install php8.0-fpm
```
```
php -v
```
```
systemctl status php8.0-fpm
```

## Install Curl
```
sudo apt update && sudo apt upgrade
sudo apt install curl
sudo apt-cache search libcurl | grep python
sudo apt install python3-pycurl
sudo apt-cache search libcurl
```

## Install PHP and Composer

```
sudo apt-get install php8.0-mysql php8.0-mbstring php8.0-xml php8.0-bcmath
sudo curl -s https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
sudo curl -s https://getcomposer.org/installer | php
```

## Laravel install:

```
sudo composer global require laravel/installer
```

## Mysql:

```
sudo apt update
sudo apt install mysql-server
sudo apt-get upgrade
sudo apt install mysql-client
sudo apt install mysql-server
```

```
sudo mysql
```
```
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password by 'your database password';
```
```
sudo mysql_secure_installation
```
```
mysql --version
```

## Install Tableplus
```
wget -qO - https://deb.tableplus.com/apt.tableplus.com.gpg.key | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://deb.tableplus.com/debian/20 tableplus main"
sudo apt update
sudo apt install tableplus
```
## Create New Database for show created Databases
```
mysql -u root -p
create database databasename;
show databases;
```

## Unlock Folder and give all permission to the folder(RWE)

### NB: place the command with conscious alert

```
sudo chmod 777 -R /var/www/html
```

## NB: place the command with conscious alert

### Migration driver not found error

```
sudo apt-get install php-mysql
```

## Composer installation or update error on project

```
composer install --ignore-platform-reqs
```

## Remove application from ubuntu linux

```
sudo apt-get remove package-name
```

## Hide mounted drive form the dock

```
gsettings set org.gnome.shell.extensions.dash-to-dock show-mounts false
```

## re-enable mounted drives on the Ubuntu Dock in future

```
gsettings set org.gnome.shell.extensions.dash-to-dock show-mounts true
```

## Customize the terminal ubuntu

## Follow this docks line by line

```
https://www.youtube.com/watch?v=PZTLIVQxxEY&t=667s&ab_channel=MuhammadbinYusrat
```

## Author: Hayatunnabi Nabil
