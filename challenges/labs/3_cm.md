
[ec2-user@ip-172-31-12-110 ~]$ hdfs dfs -ls /user
Found 8 items
drwxr-xr-x   - admin   admin               0 2017-04-07 14:01 /user/admin
drwxr-xr-x   - hdfs    supergroup          0 2017-04-07 14:01 /user/hdfs
drwxrwxrwx   - mapred  hadoop              0 2017-04-07 12:51 /user/history
drwxrwxr-t   - hive    hive                0 2017-04-07 12:52 /user/hive
drwxrwxr-x   - hue     hue                 0 2017-04-07 14:01 /user/hue
drwxr-xr-x   - neymar  neymar              0 2017-04-07 14:04 /user/neymar
drwxrwxr-x   - oozie   oozie               0 2017-04-07 12:53 /user/oozie
drwxr-xr-x   - ronaldo ronaldo             0 2017-04-07 14:05 /user/ronaldo



[ec2-user@ip-172-31-12-110 ~]$ curl -u "admin:admin" -i  http://35.160.181.143:7180/api/v14/hosts
HTTP/1.1 200 OK
Expires: Thu, 01-Jan-1970 00:00:00 GMT
Set-Cookie: CLOUDERA_MANAGER_SESSIONID=1xeqku7jxvaffsy3zuqwuqg90;Path=/;HttpOnly
Content-Type: application/json
Date: Fri, 07 Apr 2017 18:08:44 GMT
Transfer-Encoding: chunked
Server: Jetty(6.1.26.cloudera.4)

{
  "items" : [ {
    "hostId" : "f915bbfe-8dc8-4c70-ac43-0b1748441cdf",
    "ipAddress" : "172.31.10.235",
    "hostname" : "ip-172-31-10-235.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-235.us-west-2.compute.internal:7180/cmf/hostRedirect/f915bbfe-8dc8-4c70-ac43-0b1748441cdf",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "92b225db-87d5-4889-895b-956d6a10ea0c",
    "ipAddress" : "172.31.12.110",
    "hostname" : "ip-172-31-12-110.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-235.us-west-2.compute.internal:7180/cmf/hostRedirect/92b225db-87d5-4889-895b-956d6a10ea0c",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "4328395f-5e0d-4883-83cc-617780305ca7",
    "ipAddress" : "172.31.7.188",
    "hostname" : "ip-172-31-7-188.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-235.us-west-2.compute.internal:7180/cmf/hostRedirect/4328395f-5e0d-4883-83cc-617780305ca7",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "c5daf61e-1c2e-4259-abb0-1fcbffccfe21",
    "ipAddress" : "172.31.7.22",
    "hostname" : "ip-172-31-7-22.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-235.us-west-2.compute.internal:7180/cmf/hostRedirect/c5daf61e-1c2e-4259-abb0-1fcbffccfe21",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "c1ef4d7f-70d6-4215-a810-91a601d06b1f",
    "ipAddress" : "172.31.9.132",
    "hostname" : "ip-172-31-9-132.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-235.us-west-2.compute.internal:7180/cmf/hostRedirect/c1ef4d7f-70d6-4215-a810-91a601d06b1f",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  } ]
}[ec2-user@ip-172-31-12-110 ~]$
