## How to install apache2 server on linux 
- How to install apache2 server step by step 
```
sudo apt-get install apache2
sudo apt-get install php libapache2-mod-php
php -v

cd /var/www/html/
ls -la
create index.php file
sudo apt-get install vim
sudo vim index.php
sudo gedit /etc/apache2/mods-available/dir.conf
sudo chown ali:ali -R ./
sudo gedit /etc/apache2/envvars
change your user name "www" and replace "ali"

Mysql and phpmyadmin
sudo apt-get install mysql
sudo apt-get install phpmyadmin
sudo mysql

```
