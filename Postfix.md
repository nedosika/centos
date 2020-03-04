## Postfix, mysql, dovecot

1. Set your hostname:
hostnamectl set-hostname [yourhostname]

2. Edit /etc/hosts:
  AAA.BBB.CCC.DDD yourhostname.yourdomain.com       yourhostname

3. Install packages:
yum update && yum install httpd httpd-devel postfix dovecot dovecot-mysql spamassassin clamav clamav-scanner clamav-scanner-systemd clamav-data clamav-update mariadb mariadb-server php phpMyAdmin

4. Add new user to mysql:
MariaDB [(none)]> CREATE USER 'dba'@'localhost' IDENTIFIED BY 'YourPasswordHere';
MariaDB [(none)]> GRANT ALL PRIVILEGES ON * . * TO 'dba'@'localhost';
MariaDB [(none)]> FLUSH PRIVILEGES;

5. Install OpenSSL connection: 
yum install openssl mod_nss crypto-utils
yum remove mod_ssl

6. Edit NSS:
/etc/httpd/conf.d/nss.conf
Listen 443
VirtualHost _default_:443

