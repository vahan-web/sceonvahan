Server automation for a php project with Nginx, MySQL.

This script automates the following tasks:

Installation of the following services and extensions:
PHP with required extensions (e.g. MySQL, Xml etc) and composer
Nginx
MySQL Serrver and Client
Removes the default nginx vhost file
Updates a vhost file
Creates new non root low privileged user


Installation and running

Clone the repository: 
cd to project and do 'vagrant up' command
Run the following command to automate the server setup: ansible-playbook -i hosts site.yml

//it works ,but i have some problems with ansible provisioning 

PLAY [lemp] *****************************************************************************************************************************************************************

TASK [Gathering Facts] ******************************************************************************************************************************************************
fatal: [lemp]: FAILED! => {"msg": "to use the 'ssh' connection type with passwords, you must install the sshpass program"}

PLAY RECAP ******************************************************************************************************************************************************************
lemp                       : ok=0    changed=0    unreachable=0    failed=1    skipped=0    rescued=0    ignored=0   
