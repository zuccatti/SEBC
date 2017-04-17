I'm using AWS
Linux version RHEL 7.3.
Evidence from node 1
[ec2-user@ip-172-31-33-109 ~]$ uname -a
Linux ip-172-31-33-109.us-west-2.compute.internal 3.10.0-514.el7.x86_64 #1 SMP Wed Oct 19 11:24:13 EDT 2016 x86_64 x86_64 x86_64 GNU/Linux

------------------

ip-172-31-33-109.us-west-2.compute.internal
172.31.33.109
[ec2-user@ip-172-31-33-109 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  979M   40G   3% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
tmpfs           1.5G     0  1.5G   0% /run/user/0
/dev/xvdb        40G   33M   40G   1% /data



ip-172-31-42-206.us-west-2.compute.internal
172.31.42.206
[ec2-user@ip-172-31-42-206 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  980M   40G   3% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
tmpfs           1.5G     0  1.5G   0% /run/user/0
/dev/xvdb        40G   33M   40G   1% /data


ip-172-31-38-240.us-west-2.compute.internal
172.31.38.240
[ec2-user@ip-172-31-38-240 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  980M   40G   3% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
tmpfs           1.5G     0  1.5G   0% /run/user/0
/dev/xvdb        40G   33M   40G   1% /data


ip-172-31-39-159.us-west-2.compute.internal
172.31.39.159
[ec2-user@ip-172-31-39-159 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  980M   40G   3% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
tmpfs           1.5G     0  1.5G   0% /run/user/0
/dev/xvdb        40G   33M   40G   1% /data


ip-172-31-45-116.us-west-2.compute.internal
172.31.45.116
[ec2-user@ip-172-31-45-116 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  979M   40G   3% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
tmpfs           1.5G     0  1.5G   0% /run/user/0
/dev/xvdb        40G   33M   40G   1% /data

-----------------------------------

[ec2-user@ip-172-31-33-109 ~]$ sudo yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
rhui-REGION-client-config-server-7                      | 2.9 kB     00:00
rhui-REGION-rhel-server-releases                        | 3.5 kB     00:00
rhui-REGION-rhel-server-rh-common                       | 3.8 kB     00:00
(1/7): rhui-REGION-client-config-server-7/x86_64/primary_ | 5.4 kB   00:00
(2/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/g |  104 B   00:00
(3/7): rhui-REGION-rhel-server-releases/7Server/x86_64/gr | 701 kB   00:00
(4/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/u |  32 kB   00:00
(5/7): rhui-REGION-rhel-server-releases/7Server/x86_64/up | 1.9 MB   00:00
(6/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/p | 117 kB   00:00
(7/7): rhui-REGION-rhel-server-releases/7Server/x86_64/pr |  35 MB   00:00
repo id                                          repo name               status
rhui-REGION-client-config-server-7/x86_64        Red Hat Update Infrastr      6
rhui-REGION-rhel-server-releases/7Server/x86_64  Red Hat Enterprise Linu 14,232
rhui-REGION-rhel-server-rh-common/7Server/x86_64 Red Hat Enterprise Linu    225
repolist: 14,463
[ec2-user@ip-172-31-33-109 ~]$


------------------

[ec2-user@ip-172-31-33-109 ~]$ cat /etc/passwd | egrep "neymar|ronaldo"
neymar:x:2010:2010::/home/neymar:/bin/bash
ronaldo:x:2016:2016::/home/ronaldo:/bin/bash
[ec2-user@ip-172-31-33-109 ~]$ cat /etc/group | egrep "barca|meren"
barca:x:1001:neymar
merengues:x:1002:ronaldo




