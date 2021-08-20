# All-in-one OpenStack deployer

Deploy AIO OpenStack victoria on CentOS 8 Stream.

1, The environment likes follows:
a, Network:
    eth0|192.168.122.212
+-----------+-------------------+
|[ AIO Node on CentOS 8 Stream] |
+-------------------------------+
   eth1|(UP with no IP)

b, 'admin' user can sudo without a password:
admin ALL=(ALL) NOPASSWD: ALL

c, 'admin' user can ssh passwordless
-rw-------. 1 admin admin 82 Aug 20 14:38 /home/admin/.ssh/authorized_keys

2, Run ansible playbook:

$ ansible-playbook playbook.yml -i site.yml
