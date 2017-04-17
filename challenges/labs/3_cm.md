[ec2-user@ip-172-31-38-240 ~]$ hdfs dfs -ls /user
Found 8 items
drwxr-xr-x   - admin   admin               0 2017-04-17 15:05 /user/admin
drwxr-xr-x   - hdfs    supergroup          0 2017-04-17 15:05 /user/hdfs
drwxrwxrwx   - mapred  hadoop              0 2017-04-17 15:00 /user/history
drwxrwxr-t   - hive    hive                0 2017-04-17 15:01 /user/hive
drwxrwxr-x   - hue     hue                 0 2017-04-17 15:02 /user/hue
drwxr-xr-x   - neymar  neymar              0 2017-04-17 15:06 /user/neymar
drwxrwxr-x   - oozie   oozie               0 2017-04-17 15:02 /user/oozie
drwxr-xr-x   - ronaldo ronaldo             0 2017-04-17 15:06 /user/ronaldo


[ec2-user@ip-172-31-38-240 ~]$  curl -u "admin:admin" -i http://ip-172-31-42-206.us-west-2.compute.internal:7180/api/v14/hosts
HTTP/1.1 200 OK
Expires: Thu, 01-Jan-1970 00:00:00 GMT
Set-Cookie: CLOUDERA_MANAGER_SESSIONID=vtk3pduyu8jw13i1vw9i6q1l7;Path=/;HttpOnly
Content-Type: application/json
Date: Mon, 17 Apr 2017 19:08:25 GMT
Transfer-Encoding: chunked
Server: Jetty(6.1.26.cloudera.4)

{
  "items" : [ {
    "hostId" : "i-0e711de85a642c62f",
    "ipAddress" : "172.31.33.109",
    "hostname" : "ip-172-31-33-109.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-42-206.us-west-2.compute.internal:7180/cmf/hostRedirect/i-0e711de85a642c62f",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "i-05bac2af8d210ae4c",
    "ipAddress" : "172.31.38.240",
    "hostname" : "ip-172-31-38-240.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-42-206.us-west-2.compute.internal:7180/cmf/hostRedirect/i-05bac2af8d210ae4c",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "i-052f0d3e3e9b10832",
    "ipAddress" : "172.31.39.159",
    "hostname" : "ip-172-31-39-159.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-42-206.us-west-2.compute.internal:7180/cmf/hostRedirect/i-052f0d3e3e9b10832",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "3e714f96-50bc-473a-80bb-90de2bd56a0d",
    "ipAddress" : "172.31.42.206",
    "hostname" : "ip-172-31-42-206.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-42-206.us-west-2.compute.internal:7180/cmf/hostRedirect/3e714f96-50bc-473a-80bb-90de2bd56a0d",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "i-02b052a7aecdfaa47",
    "ipAddress" : "172.31.45.116",
    "hostname" : "ip-172-31-45-116.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-42-206.us-west-2.compute.internal:7180/cmf/hostRedirect/i-02b052a7aecdfaa47",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  } ]
}[ec2-user@ip-172-31-38-240 ~]$
