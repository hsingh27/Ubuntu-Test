# Ubuntu-Test
Kinetics Graduate rotation test

Date: 04/05/2016
Name: Himanshu Singh
Email: himanshu.singh@travisperkins.co.uk


I firstly created 2 VMs on Google compute, one for the Ansible control server and other as an Ubuntu test server.

Installed ansible and set up ssh keys between the ansible control server and ubuntu test server.

Configured the Ansible hosts file

I put the ansible hosts file and ansible.cfg file in the same folder as my playbook as I find it easier to modify it here rather than going to /etc/ansible/ directory

Created test.yml playbook which will first update the the package lists from the repositories and install the newest versions of all packages currently installed on the Ubuntu test server.

Only If something is updated or installed it will then reboot the ubuntu test server, wait for server to come back and once the server is restarted it will get the server uptime. 
