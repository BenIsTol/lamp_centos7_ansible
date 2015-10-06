This is a playbook will configure the lamp stack on centos 7
It can be used to configure a single node but you can modify it to work on
several nodes.
Remember you should have your ssh keys set up.
Modify the hosts file to fit your needs.
```
[webservers]
host1

[dbservers]
host2
```

Here the webserver would be configured on host1 and the dbserver on a
host2. The stack can be deployed using the following command:

```ansible-playbook -i hosts site.yml```

If you do __not__ have ssh-keys setup then you can do something like this.

```ansible-playbook -k -u <name> -i hosts site.yml```

- ```-k``` -- Will ask for password instead of key-based auth.

- ```-u``` -- Log onto the server using specified user.

If you do not have your ssh-keys setup then you might need to install
sshpass.
```yum install sshpass
```

This playbook is my first one I will get better!
