- What is ubertask optimization?
It is a way for hadoop to run "sufficiently small" faster.
Instead of creating different containers for maps and reducers, it uses only 1 JVM to to all the job.

- Where in CM is the Kerberos Security Realm value displayed?
Cloudera Manager Admin Console > Administration > Settings
Select Kerberos Category
Kerberos Security Realm will appear on the right side

- Which CDH service(s) host a property for enabling Kerberos authentication?
YARN, HDFS, Hive, MapReduce, Ooozie, Hue, Zookeeper

- How do you upgrade the CM agents?
Cloudera Manager upgrade wizard can upgrade the agent software, 
or you can install the agent and JDK software manually. 

- Give the tsquery statement used to chart Hue's CPU utilization?
select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName=hue

- Name all the roles that make up the Hive service
HiveServer2, Hive Metastore Server, WebHCat Server, Gateway

- What steps must be completed before integrating Cloudera Manager with Kerberos?
install kerberos packages
Set up a dedicated Kerberos Domain Controller
check network (FQDN lowercase; reverse lookup working; set /etc/hosts, if necessary)
