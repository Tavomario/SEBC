A command and output that shows the hostname of your database server
ANSWER:
[root@ip-172-31-42-113 share]# hostname
ip-172-31-42-113.us-west-2.compute.internal

A command and output that reports the database server version
ANSWER:
[root@ip-172-31-42-113 share]# rpm -qa | grep mariadb-server
mariadb-server-5.5.52-1.el7.x86_64

A command and output that lists all the databases in the server
ANSWER:
[root@ip-172-31-42-113 share]# mysql -u root -p
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 10
Server version: 5.5.52-MariaDB MariaDB Server

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
+--------------------+
8 rows in set (0.00 sec)

