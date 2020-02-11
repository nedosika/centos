## Opening Ports and Closing Others
1. ip a - show my ip
2. sudo firewall-cmd --list-all - show opened services
3. sudo firewall-cmd --remove-service=ssh --permanent - disabling service(ssh)
4. sudo firewall-cmd --add-service=http --permanent - open ports
5. sudo firewall-cmd --reload - reloading firewall

## Stop/Disable firewall
systemctl disable firewalld
systemctl stop firewalld
