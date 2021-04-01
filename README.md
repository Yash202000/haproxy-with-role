# haproxy-with-role

This Repository contain 2 configuratino file 1 local inventory file with ansible configuration file.

## Info about roles
### ec2-provision
This role will by default launch 3 instances over AWS cloud.

#### Note: edit ec2-provision/vars/main.yml 
var/main.yml contain configuration details with user information such access key and secret key. ensure that you will fill this information before using roles.

### myapache
This role will install apache-httpd and php in web instances 
#### Note: edit files/index.php file 
index.php file contain php code you can replace this file with index.html with your contents.

### myloadbalancer
This role will configure Haproxy server  first instance in web group other remaining instances will be configured as webservers.
