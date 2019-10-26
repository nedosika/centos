## Install Apache
1. sudo yum install httpd
2. sudo systemctl start httpd.service
3. sudo systemctl enable httpd.service

## Open Firewall
1. sudo firewall-cmd --add-service=http --permanent
2. sudo firewall-cmd --reload

## Install MySQL (MariaDB)
1. sudo yum install mariadb-server mariadb
2. sudo systemctl start mariadb
3. sudo mysql_secure_installation - enter empty password. After input new root password

## Install PHP
1. sudo yum install php php-mysql
2. sudo systemctl restart httpd.service

## install phpmyadmin
sudo yum install epel-release
sudo yum install phpmyadmin
sudo nano /etc/httpd/conf.d/phpMyAdmin.conf - add permission
sudo systemctl restart httpd.service
