[ec2-user@ip-172-31-38-240 ~]$ su ronaldo
Password:
[ronaldo@ip-172-31-38-240 ec2-user]$ kinit
Password for ronaldo@ZUCCATTI.ES:
[ronaldo@ip-172-31-38-240 ec2-user]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 10 100
Number of Maps  = 10
Samples per Map = 100
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Starting Job
17/04/17 16:59:55 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-33-109.us-west-2.compute.internal/172.31.33.109:8032
17/04/17 16:59:55 INFO hdfs.DFSClient: Created token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@ZUCCATTI.ES, renewer=yarn, realUser=, issueDate=1492462795367, maxDate=1493067595367, sequenceNumber=6, masterKeyId=2 on 172.31.33.109:8020
17/04/17 16:59:55 INFO security.TokenCache: Got dt for hdfs://ip-172-31-33-109.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.109:8020, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@ZUCCATTI.ES, renewer=yarn, realUser=, issueDate=1492462795367, maxDate=1493067595367, sequenceNumber=6, masterKeyId=2)
17/04/17 16:59:55 INFO input.FileInputFormat: Total input paths to process : 10
17/04/17 16:59:55 INFO mapreduce.JobSubmitter: number of splits:10
17/04/17 16:59:55 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492459820743_0006
17/04/17 16:59:55 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.109:8020, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@ZUCCATTI.ES, renewer=yarn, realUser=, issueDate=1492462795367, maxDate=1493067595367, sequenceNumber=6, masterKeyId=2)
17/04/17 16:59:56 INFO impl.YarnClientImpl: Submitted application application_1492459820743_0006
17/04/17 16:59:56 INFO mapreduce.Job: The url to track the job: http://ip-172-31-33-109.us-west-2.compute.internal:8088/proxy/application_1492459820743_0006/
17/04/17 16:59:56 INFO mapreduce.Job: Running job: job_1492459820743_0006
17/04/17 17:00:04 INFO mapreduce.Job: Job job_1492459820743_0006 running in uber mode : false
17/04/17 17:00:04 INFO mapreduce.Job:  map 0% reduce 0%
17/04/17 17:00:11 INFO mapreduce.Job:  map 20% reduce 0%
17/04/17 17:00:15 INFO mapreduce.Job:  map 30% reduce 0%
17/04/17 17:00:17 INFO mapreduce.Job:  map 50% reduce 0%
17/04/17 17:00:18 INFO mapreduce.Job:  map 60% reduce 0%
17/04/17 17:00:20 INFO mapreduce.Job:  map 90% reduce 0%
17/04/17 17:00:21 INFO mapreduce.Job:  map 100% reduce 0%
17/04/17 17:00:26 INFO mapreduce.Job:  map 100% reduce 100%
17/04/17 17:00:26 INFO mapreduce.Job: Job job_1492459820743_0006 completed successfully
17/04/17 17:00:27 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=88
                FILE: Number of bytes written=1369589
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=3000
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=43
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=10
                Launched reduce tasks=1
                Data-local map tasks=10
                Total time spent by all maps in occupied slots (ms)=103020
                Total time spent by all reduces in occupied slots (ms)=3407
                Total time spent by all map tasks (ms)=103020
                Total time spent by all reduce tasks (ms)=3407
                Total vcore-seconds taken by all map tasks=103020
                Total vcore-seconds taken by all reduce tasks=3407
                Total megabyte-seconds taken by all map tasks=105492480
                Total megabyte-seconds taken by all reduce tasks=3488768
        Map-Reduce Framework
                Map input records=10
                Map output records=20
                Map output bytes=180
                Map output materialized bytes=340
                Input split bytes=1820
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=340
                Reduce input records=20
                Reduce output records=0
                Spilled Records=40
                Shuffled Maps =10
                Failed Shuffles=0
                Merged Map outputs=10
                GC time elapsed (ms)=497
                CPU time spent (ms)=7100
                Physical memory (bytes) snapshot=4767055872
                Virtual memory (bytes) snapshot=17348710400
                Total committed heap usage (bytes)=5517082624
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=1180
        File Output Format Counters
                Bytes Written=97
Job Finished in 31.948 seconds
Estimated value of Pi is 3.14800000000000000000
[ronaldo@ip-172-31-38-240 ec2-user]$
