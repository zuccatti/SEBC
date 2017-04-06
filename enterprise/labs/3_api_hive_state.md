curl -u "zuccatti:cloudera" -i  http://35.163.214.52:7180/api/v1/clusters/zuccatti/services/hive/commands/start
curl -u "zuccatti:cloudera" -i  http://35.163.214.52:7180/api/v1/clusters/zuccatti/services/hive/commands/stop
curl -u "zuccatti:cloudera" -i  http://35.163.214.52:7180/api/v1/clusters/zuccatti/services/hive | grep serviceState
