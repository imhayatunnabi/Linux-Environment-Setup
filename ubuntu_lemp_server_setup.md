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

## Brave browser

```
sudo apt install -y apt-transport-https curl
```

```
curl -s https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg | sudo gpg --dearmor -o /usr/share/keyrings/brave-browser-archive-keyring.gpg
```

```
echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main" | sudo tee /etc/apt/sources.list.d/brave-browser-release.list
```

```
sudo apt update
sudo apt install -y brave-browser
```

## Discord

```
sudo apt update
sudo apt install -y snapd
sudo snap install discord
```

## Install php storm:

## Install snap beforehand:

```
sudo apt-get install snapd
```
```
sudo snap install phpstorm --classic
```

## VS Code

```
sudo apt-get install -y wget gpg
```

```
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo install -D -o root -g root -m 644 microsoft.gpg /usr/share/keyrings/microsoft.gpg
rm -f microsoft.gpg
```

```
echo "Types: deb
URIs: https://packages.microsoft.com/repos/code
Suites: stable
Components: main
Architectures: amd64,arm64,armhf
Signed-By: /usr/share/keyrings/microsoft.gpg" | sudo tee /etc/apt/sources.list.d/vscode.sources
```

```
sudo apt install -y apt-transport-https
sudo apt update
sudo apt install -y code
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

## PostgreSQL

```
sudo apt update
sudo apt install -y postgresql postgresql-contrib
sudo systemctl start postgresql
sudo systemctl enable postgresql
```

```
sudo -u postgres psql
```

```
ALTER USER postgres PASSWORD 'your_postgres_password';
\q
```

```
psql --version
```

## Redis

```
sudo apt update
sudo apt install -y redis-server
sudo systemctl start redis-server
sudo systemctl enable redis-server
```

```
redis-cli ping
```
Expected response: `PONG`

```
redis-server --version
```

## Python3 and pip

```
sudo apt update
sudo apt install -y python3 python3-pip python3-venv
```

```
python3 --version
pip3 --version
```

## Node.js with NVM

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.4/install.sh | bash
```

```
source ~/.bashrc
```
or if using zsh:
```
source ~/.zshrc
```

```
nvm install --lts
nvm use --lts
nvm alias default node
```

```
node --version
npm --version
```

## Install Tableplus
```
wget -qO - https://deb.tableplus.com/apt.tableplus.com.gpg.key | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://deb.tableplus.com/debian/20 tableplus main"
sudo apt update
sudo apt install tableplus
```

## Cursor IDE

```
sudo apt update
sudo apt install -y libfuse2
```

```
wget "https://downloader.cursor.sh/linux/appImage/x64" -O cursor.AppImage
chmod +x cursor.AppImage
./cursor.AppImage --no-sandbox
```

Optional: add to `~/.bashrc` or `~/.zshrc`:
```
alias cursor='~/cursor.AppImage --no-sandbox'
```

## pgAdmin

```
curl -fsS https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo gpg --dearmor -o /usr/share/keyrings/packages-pgadmin-org.gpg
```

```
sudo sh -c 'echo "deb [signed-by=/usr/share/keyrings/packages-pgadmin-org.gpg] https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list'
```

```
sudo apt update
sudo apt install -y pgadmin4-desktop
```

## DBeaver Studio

```
sudo apt update
sudo apt install -y snapd
sudo snap install dbeaver-ce
```

For DBeaver Ultimate/Team, download the .deb from https://dbeaver.com/download and install:
```
sudo dpkg -i dbeaver-*.deb
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
