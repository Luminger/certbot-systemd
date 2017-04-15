# certbot-systemd
systemd service for automatic letsencrypt renewals

The timer unit should be enabled.

To trigger certificate reloads 'downstream', add dependencies to your other
services (even stock services). 
https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/7/html/System_Administrators_Guide/sect-Managing_Services_with_systemd-Unit_Files.htm
