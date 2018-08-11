# Kickstart
Automate Deployment of rhel7 by booting from PXE using Kickstart file.

### Packages to be installed : 

* httpd
* xinted
* dnsmasq
* tftp-server
* syslinux

After installing all these packages, start and enable the following services using following commands:

> systemctl enable --now httpd
> systemctl enable --now xinetd
> systemctl enable --now dnsmasq

After any changes in configuration files, services needs to be restarted. 
