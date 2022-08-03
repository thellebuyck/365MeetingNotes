# NGINX Configuration Steps for RHEL 7

Below are the instructions for setting up and configuring NGINX on RHEL7.

## Commands

Run the following commands to configure nginx on RHEL.

1. This command installs ngix.  You do need to specify a version for the command. It will install nginx to specific location /opt/rh/rh-nginx112.

```yum install rh-nginx112-nginx.x86_64```

2. The configuration location /etc/opt/rh/rh-nginx112/nginx/nginx.conf
1. Service name to start:
systemctl enable rh-nginx112-nginx
systemctl start rh-nginx112-nginx