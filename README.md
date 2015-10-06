This is a playbook will configure the lamp stack on centos 7
It can be used to configure a single node or multiple nodes.

Modify the hosts file to fit your needs.

        [webservers]
        host1

        [dbservers]
        host2

Here the webserver would be configured on host1 and the dbserver on a
host2. The stack can be deployed using the following command:

        ansible-playbook -i hosts site.yml

This is my first playbook I will get better!
