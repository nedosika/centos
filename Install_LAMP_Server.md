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
1. sudo yum install epel-release
2. sudo yum install phpmyadmin
3. sudo nano /etc/httpd/conf.d/phpMyAdmin.conf - add permission
4. sudo systemctl restart httpd.service
