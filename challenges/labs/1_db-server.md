MariaDB [(none)]> show variables like 'hostname';
+---------------+---------------------------------------------+
| Variable_name | Value                                       |
+---------------+---------------------------------------------+
| hostname      | ip-172-31-33-109.us-west-2.compute.internal |
+---------------+---------------------------------------------+
1 row in set (0.00 sec)

MariaDB [(none)]> SELECT @@version;
+----------------------+
| @@version            |
+----------------------+
| 5.5.54-MariaDB-wsrep |
+----------------------+
1 row in set (0.00 sec)

MariaDB [(none)]> show databases
    -> ;
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
| sentry             |
+--------------------+
11 rows in set (0.00 sec)



