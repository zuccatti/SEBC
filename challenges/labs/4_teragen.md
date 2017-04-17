[ec2-user@ip-172-31-38-240 ~]$ su neymar
Password:
[neymar@ip-172-31-38-240 ec2-user]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen  -Ddfs.blocksize=16777216 65536000 tgen640
17/04/17 15:15:51 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-33-109.us-west-2.compute.internal/172.31.33.109:8032
17/04/17 15:15:51 INFO terasort.TeraSort: Generating 65536000 using 2
17/04/17 15:15:51 INFO mapreduce.JobSubmitter: number of splits:2
17/04/17 15:15:51 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492455639669_0001
17/04/17 15:15:52 INFO impl.YarnClientImpl: Submitted application application_1492455639669_0001
17/04/17 15:15:52 INFO mapreduce.Job: The url to track the job: http://ip-172-31-33-109.us-west-2.compute.internal:8088/proxy/application_1492455639669_0001/
17/04/17 15:15:52 INFO mapreduce.Job: Running job: job_1492455639669_0001
17/04/17 15:15:59 INFO mapreduce.Job: Job job_1492455639669_0001 running in uber mode : false
17/04/17 15:15:59 INFO mapreduce.Job:  map 0% reduce 0%
17/04/17 15:16:11 INFO mapreduce.Job:  map 5% reduce 0%
17/04/17 15:16:12 INFO mapreduce.Job:  map 10% reduce 0%
17/04/17 15:16:15 INFO mapreduce.Job:  map 16% reduce 0%
17/04/17 15:16:18 INFO mapreduce.Job:  map 21% reduce 0%
17/04/17 15:16:21 INFO mapreduce.Job:  map 24% reduce 0%
17/04/17 15:16:24 INFO mapreduce.Job:  map 26% reduce 0%
17/04/17 15:16:27 INFO mapreduce.Job:  map 29% reduce 0%
17/04/17 15:16:30 INFO mapreduce.Job:  map 31% reduce 0%
17/04/17 15:16:33 INFO mapreduce.Job:  map 34% reduce 0%
17/04/17 15:16:37 INFO mapreduce.Job:  map 36% reduce 0%
17/04/17 15:16:40 INFO mapreduce.Job:  map 40% reduce 0%
17/04/17 15:16:43 INFO mapreduce.Job:  map 43% reduce 0%
17/04/17 15:16:46 INFO mapreduce.Job:  map 46% reduce 0%
17/04/17 15:16:49 INFO mapreduce.Job:  map 48% reduce 0%
17/04/17 15:16:52 INFO mapreduce.Job:  map 50% reduce 0%
17/04/17 15:16:55 INFO mapreduce.Job:  map 53% reduce 0%
17/04/17 15:16:58 INFO mapreduce.Job:  map 56% reduce 0%
17/04/17 15:17:01 INFO mapreduce.Job:  map 60% reduce 0%
17/04/17 15:17:04 INFO mapreduce.Job:  map 63% reduce 0%
17/04/17 15:17:07 INFO mapreduce.Job:  map 66% reduce 0%
17/04/17 15:17:10 INFO mapreduce.Job:  map 68% reduce 0%
17/04/17 15:17:13 INFO mapreduce.Job:  map 71% reduce 0%
17/04/17 15:17:16 INFO mapreduce.Job:  map 74% reduce 0%
17/04/17 15:17:19 INFO mapreduce.Job:  map 76% reduce 0%
17/04/17 15:17:22 INFO mapreduce.Job:  map 80% reduce 0%
17/04/17 15:17:25 INFO mapreduce.Job:  map 83% reduce 0%
17/04/17 15:17:28 INFO mapreduce.Job:  map 86% reduce 0%
17/04/17 15:17:31 INFO mapreduce.Job:  map 88% reduce 0%
17/04/17 15:17:34 INFO mapreduce.Job:  map 90% reduce 0%
17/04/17 15:17:37 INFO mapreduce.Job:  map 93% reduce 0%
17/04/17 15:17:40 INFO mapreduce.Job:  map 96% reduce 0%
17/04/17 15:17:43 INFO mapreduce.Job:  map 99% reduce 0%
17/04/17 15:17:45 INFO mapreduce.Job:  map 100% reduce 0%
17/04/17 15:17:45 INFO mapreduce.Job: Job job_1492455639669_0001 completed successfully
17/04/17 15:17:45 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=246052
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=170
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=8
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=4
        Job Counters
                Launched map tasks=2
                Other local map tasks=2
                Total time spent by all maps in occupied slots (ms)=205931
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=205931
                Total vcore-seconds taken by all map tasks=205931
                Total megabyte-seconds taken by all map tasks=210873344
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=170
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=914
                CPU time spent (ms)=102370
                Physical memory (bytes) snapshot=410992640
                Virtual memory (bytes) snapshot=3166052352
                Total committed heap usage (bytes)=420478976
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    1m56.652s
user    0m5.749s
sys     0m0.282s
[neymar@ip-172-31-38-240 ec2-user]$

------------------------------

[neymar@ip-172-31-38-240 ec2-user]$ hdfs dfs -ls /user/neymar/tgen640
Found 3 items
-rw-r--r--   3 neymar neymar          0 2017-04-17 15:17 /user/neymar/tgen640/_SUCCESS
-rw-r--r--   3 neymar neymar 3276800000 2017-04-17 15:17 /user/neymar/tgen640/part-m-00000
-rw-r--r--   3 neymar neymar 3276800000 2017-04-17 15:17 /user/neymar/tgen640/part-m-00001


------------------------------

[neymar@ip-172-31-38-240 ec2-user]$ hdfs fsck /user/neymar/tgen640 -blocks
Connecting to namenode via http://ip-172-31-33-109.us-west-2.compute.internal:50070
FSCK started by neymar (auth:SIMPLE) from /172.31.38.240 for path /user/neymar/tgen640 at Mon Apr 17 15:20:10 EDT 2017
...Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    1
 Total files:   3
 Total symlinks:                0
 Total blocks (validated):      392 (avg. block size 16718367 B)
 Minimally replicated blocks:   392 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          3
 Number of racks:               1
FSCK ended at Mon Apr 17 15:20:10 EDT 2017 in 31 milliseconds


The filesystem under path '/user/neymar/tgen640' is HEALTHY
[neymar@ip-172-31-38-240 ec2-user]$



