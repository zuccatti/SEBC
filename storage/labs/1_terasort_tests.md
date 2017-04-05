[ec2-user@ip-172-31-15-113 ~]$ sudo su - hdfs
Last login: Wed Apr  5 19:34:52 EDT 2017 on pts/2
[hdfs@ip-172-31-15-113 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/lib/hadoop-mapreduce/hadoop-mapreduce-examples-2.6.0-cdh5.10.1.jar teragen -Ddfs.blocksize=33554432 -Dmapreduce_job_counters_limit=4  100000000 /users/zuccatti/teragen2
17/04/05 19:35:39 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-0-15.us-west-2.compute.internal/172.31.0.15:8032
17/04/05 19:35:40 INFO terasort.TeraGen: Generating 100000000 using 2
17/04/05 19:35:40 INFO mapreduce.JobSubmitter: number of splits:2
17/04/05 19:35:40 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491415082966_0006
17/04/05 19:35:40 INFO impl.YarnClientImpl: Submitted application application_1491415082966_0006
17/04/05 19:35:41 INFO mapreduce.Job: The url to track the job: http://ip-172-31-0-15.us-west-2.compute.internal:8088/proxy/application_1491415082966_0006/
17/04/05 19:35:41 INFO mapreduce.Job: Running job: job_1491415082966_0006
17/04/05 19:35:47 INFO mapreduce.Job: Job job_1491415082966_0006 running in uber mode : false
17/04/05 19:35:47 INFO mapreduce.Job:  map 0% reduce 0%
17/04/05 19:36:05 INFO mapreduce.Job:  map 13% reduce 0%
17/04/05 19:36:11 INFO mapreduce.Job:  map 17% reduce 0%
17/04/05 19:36:17 INFO mapreduce.Job:  map 20% reduce 0%
17/04/05 19:36:23 INFO mapreduce.Job:  map 22% reduce 0%
17/04/05 19:36:29 INFO mapreduce.Job:  map 26% reduce 0%
17/04/05 19:36:35 INFO mapreduce.Job:  map 30% reduce 0%
17/04/05 19:36:41 INFO mapreduce.Job:  map 34% reduce 0%
17/04/05 19:36:47 INFO mapreduce.Job:  map 37% reduce 0%
17/04/05 19:36:53 INFO mapreduce.Job:  map 41% reduce 0%
17/04/05 19:36:59 INFO mapreduce.Job:  map 45% reduce 0%
17/04/05 19:37:05 INFO mapreduce.Job:  map 49% reduce 0%
17/04/05 19:37:11 INFO mapreduce.Job:  map 51% reduce 0%
17/04/05 19:37:17 INFO mapreduce.Job:  map 55% reduce 0%
17/04/05 19:37:23 INFO mapreduce.Job:  map 60% reduce 0%
17/04/05 19:37:29 INFO mapreduce.Job:  map 63% reduce 0%
17/04/05 19:37:35 INFO mapreduce.Job:  map 67% reduce 0%
17/04/05 19:37:41 INFO mapreduce.Job:  map 71% reduce 0%
17/04/05 19:37:47 INFO mapreduce.Job:  map 74% reduce 0%
17/04/05 19:37:53 INFO mapreduce.Job:  map 78% reduce 0%
17/04/05 19:37:59 INFO mapreduce.Job:  map 82% reduce 0%
17/04/05 19:38:05 INFO mapreduce.Job:  map 86% reduce 0%
17/04/05 19:38:11 INFO mapreduce.Job:  map 89% reduce 0%
17/04/05 19:38:17 INFO mapreduce.Job:  map 93% reduce 0%
17/04/05 19:38:23 INFO mapreduce.Job:  map 97% reduce 0%
17/04/05 19:38:30 INFO mapreduce.Job:  map 100% reduce 0%
17/04/05 19:38:30 INFO mapreduce.Job: Job job_1491415082966_0006 completed successfully
17/04/05 19:38:30 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=250092
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=170
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=8
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=4
        Job Counters
                Launched map tasks=2
                Other local map tasks=2
                Total time spent by all maps in occupied slots (ms)=321471
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=321471
                Total vcore-seconds taken by all map tasks=321471
                Total megabyte-seconds taken by all map tasks=329186304
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Input split bytes=170
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1519
                CPU time spent (ms)=137480
                Physical memory (bytes) snapshot=442441728
                Virtual memory (bytes) snapshot=3155038208
                Total committed heap usage (bytes)=396361728
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=214760662691937609
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=10000000000

real    2m52.807s
user    0m6.610s
sys     0m0.338s
[hdfs@ip-172-31-15-113 ~]$ exit
logout

=============================================================

