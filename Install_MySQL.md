## Installing MySQL
1. Go to dev.mysql.com/downloads
2. wget https://dev.mysql.com/get/{mysql80-community-release-el7-3.noarch.rpm}.noarch.rpm
3. Copmarring: md5sum {mysql80-community-release-el7-3.noarch.rpm} - MD5: 893b55d5d885df5c4d4cf7c4f2f6c153
4. Install package: sudo rpm -ivh mysql57-community-release-el7-9.noarch.rpm
5. Install MySQL-serevr: sudo yum install mysql-server

## Starting MySQL
1. sudo systemctl start mysqld
2. sudo systemctl status mysqld
3. sudo systemctl disable mysqld
4. sudo grep 'temporary password' /var/log/mysqld.log

## Configuring MySQL
1. sudo mysql_secure_installation

## Testing MySQL
1. mysqladmin -u root -p version
