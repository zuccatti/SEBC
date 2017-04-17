[ec2-user@ip-172-31-42-206 ~]$  ls /etc/yum.repos.d
cloudera-manager.repo  redhat.repo  redhat-rhui-client-config.repo  redhat-rhui.repo  rhui-load-balancers.conf
[ec2-user@ip-172-31-42-206 ~]$


BEFORE REPOSYNC
[ec2-user@ip-172-31-42-206 ~]$ sudo cat /etc/yum.repos.d/cloudera-manager.repo
[cloudera-manager]
# Packages for Cloudera Manager, Version 5, on RedHat or CentOS 7 x86_64
name=Cloudera Manager
baseurl=https://archive.cloudera.com/cm5/redhat/7/x86_64/cm/5.9/
gpgkey =https://archive.cloudera.com/cm5/redhat/7/x86_64/cm/RPM-GPG-KEY-cloudera
gpgcheck = 1
[ec2-user@ip-172-31-42-206 ~]$


AFTER REPOSYNC
[ec2-user@ip-172-31-42-206 yum.repos.d]$  sudo cat /etc/yum.repos.d/cloudera-manager.repo
[cloudera-manager]
# Packages for Cloudera Manager, Version 5, on RedHat or CentOS 7 x86_64
name=Cloudera Manager
baseurl=http://ip-172-31-42-206.us-west-2.compute.internal/cm5/redhat/7/x86_64/cm/5/
gpgkey =http://ip-172-31-42-206.us-west-2.compute.internal/cm5/redhat/7/x86_64/cm/RPM-GPG-KEY-cloudera
gpgcheck = 1
[ec2-user@ip-172-31-42-206 yum.repos.d]$


[ec2-user@ip-172-31-42-206 x86_64]$ sudo /usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-33-109.us-west-2.compute.internal -u root -p scm scm scm 


