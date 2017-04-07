[hdfs@ip-172-31-12-110 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/lib/hadoop-mapreduce/hadoop-mapreduce-examples-2.6.0-cdh5.10.1.jar teragen  -Ddfs.blocksize=16777216 65536000 tgen640
17/04/07 14:25:34 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-12-110.us-west-2.compute.internal/172.31.12.110:8032
17/04/07 14:25:35 INFO terasort.TeraGen: Generating 65536000 using 2
17/04/07 14:25:35 INFO mapreduce.JobSubmitter: number of splits:2
17/04/07 14:25:35 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491589428254_0003
17/04/07 14:25:36 INFO impl.YarnClientImpl: Submitted application application_1491589428254_0003
17/04/07 14:25:36 INFO mapreduce.Job: The url to track the job: http://ip-172-31-12-110.us-west-2.compute.internal:8088/proxy/application_1491589428254_0003/
17/04/07 14:25:36 INFO mapreduce.Job: Running job: job_1491589428254_0003
17/04/07 14:25:43 INFO mapreduce.Job: Job job_1491589428254_0003 running in uber mode : false
17/04/07 14:25:43 INFO mapreduce.Job:  map 0% reduce 0%
17/04/07 14:26:03 INFO mapreduce.Job:  map 21% reduce 0%
17/04/07 14:26:09 INFO mapreduce.Job:  map 24% reduce 0%
17/04/07 14:26:10 INFO mapreduce.Job:  map 27% reduce 0%
17/04/07 14:26:15 INFO mapreduce.Job:  map 30% reduce 0%
17/04/07 14:26:16 INFO mapreduce.Job:  map 32% reduce 0%
17/04/07 14:26:21 INFO mapreduce.Job:  map 35% reduce 0%
17/04/07 14:26:22 INFO mapreduce.Job:  map 38% reduce 0%
17/04/07 14:26:28 INFO mapreduce.Job:  map 44% reduce 0%
17/04/07 14:26:34 INFO mapreduce.Job:  map 49% reduce 0%
17/04/07 14:26:40 INFO mapreduce.Job:  map 55% reduce 0%
17/04/07 14:26:46 INFO mapreduce.Job:  map 60% reduce 0%
17/04/07 14:26:52 INFO mapreduce.Job:  map 66% reduce 0%
17/04/07 14:26:58 INFO mapreduce.Job:  map 72% reduce 0%
17/04/07 14:27:04 INFO mapreduce.Job:  map 77% reduce 0%
17/04/07 14:27:10 INFO mapreduce.Job:  map 83% reduce 0%
17/04/07 14:27:16 INFO mapreduce.Job:  map 89% reduce 0%
17/04/07 14:27:22 INFO mapreduce.Job:  map 95% reduce 0%
17/04/07 14:27:27 INFO mapreduce.Job:  map 97% reduce 0%
17/04/07 14:27:28 INFO mapreduce.Job:  map 100% reduce 0%
17/04/07 14:27:28 INFO mapreduce.Job: Job job_1491589428254_0003 completed successfully
17/04/07 14:27:28 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=250088
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
                Total time spent by all maps in occupied slots (ms)=204848
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=204848
                Total vcore-seconds taken by all map tasks=204848
                Total megabyte-seconds taken by all map tasks=209764352
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=170
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1283
                CPU time spent (ms)=102240
                Physical memory (bytes) snapshot=417005568
                Virtual memory (bytes) snapshot=3153125376
                Total committed heap usage (bytes)=408944640
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    1m56.515s
user    0m6.134s
sys     0m0.277s
[hdfs@ip-172-31-12-110 ~]$




--------------------------------------


[hdfs@ip-172-31-12-110 ~]$ hdfs dfs -ls /user/neymar/tgen640
Found 3 items
-rw-r--r--   3 neymar neymar          0 2017-04-07 14:27 /user/neymar/tgen640/_SUCCESS
-rw-r--r--   3 neymar neymar 3276800000 2017-04-07 14:27 /user/neymar/tgen640/part-m-00000
-rw-r--r--   3 neymar neymar 3276800000 2017-04-07 14:27 /user/neymar/tgen640/part-m-00001


========================================


[hdfs@ip-172-31-12-110 ~]$ hdfs fsck /user/neymar/tgen640 -blocks
Connecting to namenode via http://ip-172-31-12-110.us-west-2.compute.internal:50070
FSCK started by neymar (auth:SIMPLE) from /172.31.12.110 for path /user/neymar/tgen640 at Fri Apr 07 14:31:02 EDT 2017
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
FSCK ended at Fri Apr 07 14:31:02 EDT 2017 in 15 milliseconds


The filesystem under path '/user/neymar/tgen640' is HEALTHY
