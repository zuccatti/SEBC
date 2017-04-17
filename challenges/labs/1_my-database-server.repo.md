I'm creating a local repo based on this:

[ec2-user@ip-172-31-33-109 yum.repos.d]$  sudo cat /etc/yum.repos.d/mariadb.repo
[mariadb]
name=MariaDB
baseurl=https://yum.mariadb.org/5.5.54/rhel7-amd64/
gpgkey=https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
gpgcheck=1
[ec2-user@ip-172-31-33-109 yum.repos.d]$

