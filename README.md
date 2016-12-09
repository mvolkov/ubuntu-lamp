### Apache
Create an Apache server as part of Runner training in the Centurylink Cloud

### Description
This playbook will provision an Ubuntu server, install apache, and place a configuration to proxy traffic to a backend group of your choosing. The high level tasks are:
* provision server (option public IP address)
* install apache
* place configuration
* start / enable apache

### Required
* listen port: port the apache server will listen for traffic
* backend group: CLC group of servers to send request traffic to
* backend port: port the backend servers will recieve traffic on

### Optional
* clc group: name of the CLC group
* clc server name: name of the CLC server
* public ip: default is true. If you want to prevent a public IP from provisioning, set this to false
