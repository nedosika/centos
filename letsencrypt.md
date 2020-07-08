yum install epel-release
yum install certbot python2-certbot-apache mod_ssl
certbot --apache -d example.com
certbot --apache -d example.com -d www.example.com
certbot --apache

https://www.ssllabs.com/ssltest/analyze.html?d=example.com

certbot renew --dry-run

crontab -e

crontab
0 0,12 * * * python -c 'import random; import time; time.sleep(random.random() * 3600)' && certbot renew
