
[ec2-user@ip-172-31-7-22 ~]$ hostname -f
ip-172-31-7-22.us-west-2.compute.internal


MariaDB [(none)]> SELECT @@version;
+----------------+
| @@version      |
+----------------+
| 5.5.52-MariaDB |
+----------------+
1 row in set (0.00 sec)

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| hue                |
| metastore          |
| mysql              |
| nav                |
| navms              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
12 rows in set (0.00 sec)
