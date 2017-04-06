{
  "timestamp" : "2017-04-06T16:33:37.752Z",
  "clusters" : [ {
    "name" : "zuccatti",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "654311424"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "654311424"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3432356249"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "577"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-5-7.us-west-2.compute.internal"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-334598947f3315ccc1fcad98b42a201f",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "dd601785-5c4e-4088-bf58-4fdb9401d5a4"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-862f3a7740a13fc5484881d727c09a14",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "90282f61-41a5-4c3b-81ce-22fc8d1d6843"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-adfd271441019d994ac0759e84b4c9ef",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8v8ok9uw2thej4a7n3jwvgfsf"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ddqjeey56n4ssp7t5fpsnhwuy"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "654311424"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-334598947f3315ccc1fcad98b42a201f",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "dd601785-5c4e-4088-bf58-4fdb9401d5a4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5q4a74hcjgvsa65zpk7lzg25m"
          }, {
            "name" : "serverId",
            "value" : "4"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-862f3a7740a13fc5484881d727c09a14",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "90282f61-41a5-4c3b-81ce-22fc8d1d6843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "24yn7wgc17u95ngjrvmhg3mo8"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "wbclryaazepd3uhc49aznif3"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-adfd271441019d994ac0759e84b4c9ef",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "21hauz3h19psg1y1zbeg2c2vt"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "6"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "654311424"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "rm_cpu_shares",
            "value" : "1800"
          }, {
            "name" : "rm_io_weight",
            "value" : "900"
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "3"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1024"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "654311424"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "1024"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "wXSQmbZV0Eg7RaEnCmtypuqwv4MGrI"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6nhq83pfqu3u3yx7iipnt7rza"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-334598947f3315ccc1fcad98b42a201f",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "dd601785-5c4e-4088-bf58-4fdb9401d5a4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6wesg0t98kc143zch89djb273"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-862f3a7740a13fc5484881d727c09a14",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "90282f61-41a5-4c3b-81ce-22fc8d1d6843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "elh9u5huqka5nxm55ih8kagls"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-adfd271441019d994ac0759e84b4c9ef",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "47amlm6j6bplkr9kl6d6qu5gs"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "46"
          }, {
            "name" : "role_jceks_password",
            "value" : "emrpnip07puzhsu8pttbjzlrm"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "654311424"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "4293706956"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "654311424"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "654311424"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "L5gid4u3l0ZHDqpnMCyLBRDMvNHqEE"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "RHvs2XypTRXTwt8RGi6nrG9qUovMGm"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "gm0lMxdwz8ZyvupLstHHb1Wr9xg4Fc"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-334598947f3315ccc1fcad98b42a201f",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "dd601785-5c4e-4088-bf58-4fdb9401d5a4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dvraaa6qpyzcschuuehbdjtbd"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-862f3a7740a13fc5484881d727c09a14",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "90282f61-41a5-4c3b-81ce-22fc8d1d6843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bg42mqxbewmssxpz9ou4fiook"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-adfd271441019d994ac0759e84b4c9ef",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8cwqpfcc5gzky1v299xwm5oh1"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cyrzm4d2ledvlsphtxpn7a8wt"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-adfd271441019d994ac0759e84b4c9ef",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d3i0wn9oylwx8dyigphm4kkbi"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ajbjhn72fzimwi7z583o5353i"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-adfd271441019d994ac0759e84b4c9ef",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4fjlcx15618ujgtq3oc419z7r"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-334598947f3315ccc1fcad98b42a201f",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "dd601785-5c4e-4088-bf58-4fdb9401d5a4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a0dk2sdxw479io030qdiizhhi"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-862f3a7740a13fc5484881d727c09a14",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "90282f61-41a5-4c3b-81ce-22fc8d1d6843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ddi3m1k8k4uy32q23lrvnaitz"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dveclzre4tmw7z5pkfdtbfjdm"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservicesebc"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservicesebc"
          }, {
            "name" : "namenode_id",
            "value" : "48"
          }, {
            "name" : "role_jceks_password",
            "value" : "e2ccv9788rduh3t0ckzkhlz5a"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-adfd271441019d994ac0759e84b4c9ef",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservicesebc"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservicesebc"
          }, {
            "name" : "namenode_id",
            "value" : "65"
          }, {
            "name" : "role_jceks_password",
            "value" : "grwhmsz3qvwkzq7fh4vv167h"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "mapreduce",
      "type" : "MAPREDUCE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "JOBTRACKER",
          "items" : [ {
            "name" : "jobtracker_java_heapsize",
            "value" : "52428800"
          }, {
            "name" : "jobtracker_mapred_local_dir_list",
            "value" : "/mapred/jt"
          }, {
            "name" : "mapred_job_tracker_handler_count",
            "value" : "22"
          } ]
        }, {
          "roleType" : "TASKTRACKER",
          "items" : [ {
            "name" : "mapred_tasktracker_instrumentation",
            "value" : "org.apache.hadoop.mapred.TaskTrackerCmonInst"
          }, {
            "name" : "mapred_tasktracker_map_tasks_maximum",
            "value" : "1"
          }, {
            "name" : "mapred_tasktracker_reduce_tasks_maximum",
            "value" : "1"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "20"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          }, {
            "name" : "task_tracker_java_heapsize",
            "value" : "52428800"
          }, {
            "name" : "tasktracker_mapred_local_dir_list",
            "value" : "/mapred/local,/data/mapred/local"
          } ]
        } ],
        "items" : [ {
          "name" : "fc_authorization_secret_key",
          "value" : "0Ld5Fk1r1DGwDJFWva8BxjgoiT6laq"
        }, {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "0"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "mapreduce-JOBTRACKER-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "JOBTRACKER",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "job_tracker_id",
            "value" : "57"
          }, {
            "name" : "role_jceks_password",
            "value" : "185xp56ymj9l2ell7e1zm9goz"
          } ]
        }
      }, {
        "name" : "mapreduce-TASKTRACKER-334598947f3315ccc1fcad98b42a201f",
        "type" : "TASKTRACKER",
        "hostRef" : {
          "hostId" : "dd601785-5c4e-4088-bf58-4fdb9401d5a4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ecqhqrbwytyj8fhjpobg21gma"
          } ]
        }
      }, {
        "name" : "mapreduce-TASKTRACKER-862f3a7740a13fc5484881d727c09a14",
        "type" : "TASKTRACKER",
        "hostRef" : {
          "hostId" : "90282f61-41a5-4c3b-81ce-22fc8d1d6843"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "arcbu4t821ymnoc1whe03vr7"
          } ]
        }
      }, {
        "name" : "mapreduce-TASKTRACKER-adfd271441019d994ac0759e84b4c9ef",
        "type" : "TASKTRACKER",
        "hostRef" : {
          "hostId" : "aee4a034-8948-45b2-a648-89678beacc09"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d368ewgnl4ej0zqkvu7moa6a3"
          } ]
        }
      } ],
      "displayName" : "MapReduce"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-5-7.us-west-2.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "52428800"
          } ]
        } ],
        "items" : [ {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7hocjwbe6atqn3vc36xujfqcr"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-5-7.us-west-2.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "hue"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-8ad2e925f20071de5e7dd392fce24a09"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-8ad2e925f20071de5e7dd392fce24a09",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aicbmkuibsx119w7emrkh2x9f"
          }, {
            "name" : "secret_key",
            "value" : "xO0gNsRcWSqnPKtlXACSgIsAUNuDyx"
          } ]
        }
      } ],
      "displayName" : "Hue"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd",
    "ipAddress" : "172.31.0.15",
    "hostname" : "ip-172-31-0-15.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "aee4a034-8948-45b2-a648-89678beacc09",
    "ipAddress" : "172.31.15.113",
    "hostname" : "ip-172-31-15-113.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "90282f61-41a5-4c3b-81ce-22fc8d1d6843",
    "ipAddress" : "172.31.15.21",
    "hostname" : "ip-172-31-15-21.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "dd601785-5c4e-4088-bf58-4fdb9401d5a4",
    "ipAddress" : "172.31.2.236",
    "hostname" : "ip-172-31-2-236.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "cc205d6a-8dec-4134-bc87-d0c38a4fcf36",
    "ipAddress" : "172.31.5.7",
    "hostname" : "ip-172-31-5-7.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-8ad2e925f20071de5e7dd392fce24a09",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "353476737d799c220c75efeaa2254dec1394f4abe5b74a36cc481063c0ed71a3",
    "pwSalt" : -3030488061952918346,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-8ad2e925f20071de5e7dd392fce24a09",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "1ff202fa245f20fed5f19beff738e0ff655618e6a13bc2653e725da800ebed09",
    "pwSalt" : 332820512373089250,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-8ad2e925f20071de5e7dd392fce24a09",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "49e1eda11538e0a48087f83776c01193cfef77a67c5e2524aaf19154ada37eb3",
    "pwSalt" : -3306030740661487916,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-8ad2e925f20071de5e7dd392fce24a09",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "5ce544a57c2021160c3633c40b232a3b8efb3e4fc138ba4314fd247c7754cf54",
    "pwSalt" : -2957554610547623683,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "374dc129ce26c6b4d76811f269bb8da583478d779a2a5615863f12dd6c8aca28",
    "pwSalt" : 6055937574596635,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "df187557978fcb3b87570df7c8cade817fff2e455cff49723f31e8ae60e09759",
    "pwSalt" : 2920365154943357469,
    "pwLogin" : true
  }, {
    "name" : "zuccatti",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "2eb1cdb01a2d178eb669c42abba860dd9a6fa5e9653dfc0d14cc5c6b5d02b636",
    "pwSalt" : -3752164108862170708,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.10.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170319-2001",
    "gitHash" : "f226435f6fa5f545543c00245900ae43bea7a29c",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "654311424"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "654311424"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "850395136"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-5-7.us-west-2.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "654311424"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "654311424"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "850395136"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-8ad2e925f20071de5e7dd392fce24a09",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9qenqlqq7hf3a6d3bq3u18gdv"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-8ad2e925f20071de5e7dd392fce24a09",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "edujt7vhw7e1dzvkt0mq7l5sq"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-8ad2e925f20071de5e7dd392fce24a09",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9q5kheftrnor97nsbzxh8j1ri"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-8ad2e925f20071de5e7dd392fce24a09",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ewqw9cyv2s2c5zpynym8hfz8o"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-8ad2e925f20071de5e7dd392fce24a09",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "3d489212-af47-4cee-9f60-58c6d35a1fcd"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "e39sda6idvdoytsqf2qj2qgd6"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/27/2012 21:40"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}
