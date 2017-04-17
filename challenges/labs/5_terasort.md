[ec2-user@ip-172-31-38-240 ~]$ su neymar
Password:
[neymar@ip-172-31-38-240 ec2-user]$ kinit
Password for neymar@ZUCCATTI.ES:
[neymar@ip-172-31-38-240 ec2-user]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort tgen640 tsort640
17/04/17 16:49:17 INFO terasort.TeraSort: starting
17/04/17 16:49:19 INFO hdfs.DFSClient: Created token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@ZUCCATTI.ES, renewer=yarn, realUser=, issueDate=1492462159028, maxDate=1493066959028, sequenceNumber=5, masterKeyId=2 on 172.31.33.109:8020
17/04/17 16:49:19 INFO security.TokenCache: Got dt for hdfs://ip-172-31-33-109.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.109:8020, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@ZUCCATTI.ES, renewer=yarn, realUser=, issueDate=1492462159028, maxDate=1493066959028, sequenceNumber=5, masterKeyId=2)
17/04/17 16:49:19 INFO input.FileInputFormat: Total input paths to process : 2
Spent 364ms computing base-splits.
Spent 7ms computing TeraScheduler splits.
Computing input splits took 372ms
Sampling 10 splits of 392
Making 6 from 100000 sampled records
Computing parititions took 859ms
Spent 1233ms computing partitions.
17/04/17 16:49:20 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-33-109.us-west-2.compute.internal/172.31.33.109:8032
17/04/17 16:49:20 INFO mapreduce.JobSubmitter: number of splits:392
17/04/17 16:49:20 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492459820743_0005
17/04/17 16:49:20 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.109:8020, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@ZUCCATTI.ES, renewer=yarn, realUser=, issueDate=1492462159028, maxDate=1493066959028, sequenceNumber=5, masterKeyId=2)
17/04/17 16:49:21 INFO impl.YarnClientImpl: Submitted application application_1492459820743_0005
17/04/17 16:49:21 INFO mapreduce.Job: The url to track the job: http://ip-172-31-33-109.us-west-2.compute.internal:8088/proxy/application_1492459820743_0005/
17/04/17 16:49:21 INFO mapreduce.Job: Running job: job_1492459820743_0005
17/04/17 16:49:29 INFO mapreduce.Job: Job job_1492459820743_0005 running in uber mode : false
17/04/17 16:49:29 INFO mapreduce.Job:  map 0% reduce 0%
17/04/17 16:49:41 INFO mapreduce.Job:  map 1% reduce 0%
17/04/17 16:49:45 INFO mapreduce.Job:  map 2% reduce 0%
17/04/17 16:49:50 INFO mapreduce.Job:  map 3% reduce 0%
17/04/17 16:49:54 INFO mapreduce.Job:  map 4% reduce 0%
17/04/17 16:49:55 INFO mapreduce.Job:  map 5% reduce 0%
17/04/17 16:50:01 INFO mapreduce.Job:  map 6% reduce 0%
17/04/17 16:50:05 INFO mapreduce.Job:  map 7% reduce 0%
17/04/17 16:50:09 INFO mapreduce.Job:  map 8% reduce 0%
17/04/17 16:50:14 INFO mapreduce.Job:  map 9% reduce 0%
17/04/17 16:50:18 INFO mapreduce.Job:  map 10% reduce 0%
17/04/17 16:50:22 INFO mapreduce.Job:  map 11% reduce 0%
17/04/17 16:50:27 INFO mapreduce.Job:  map 12% reduce 0%
17/04/17 16:50:28 INFO mapreduce.Job:  map 13% reduce 0%
17/04/17 16:50:34 INFO mapreduce.Job:  map 14% reduce 0%
17/04/17 16:50:36 INFO mapreduce.Job:  map 15% reduce 0%
17/04/17 16:50:42 INFO mapreduce.Job:  map 16% reduce 0%
17/04/17 16:50:44 INFO mapreduce.Job:  map 17% reduce 0%
17/04/17 16:50:50 INFO mapreduce.Job:  map 18% reduce 0%
17/04/17 16:50:53 INFO mapreduce.Job:  map 19% reduce 0%
17/04/17 16:50:57 INFO mapreduce.Job:  map 20% reduce 0%
17/04/17 16:51:02 INFO mapreduce.Job:  map 21% reduce 0%
17/04/17 16:51:03 INFO mapreduce.Job:  map 22% reduce 0%
17/04/17 16:51:09 INFO mapreduce.Job:  map 23% reduce 0%
17/04/17 16:51:12 INFO mapreduce.Job:  map 24% reduce 0%
17/04/17 16:51:18 INFO mapreduce.Job:  map 25% reduce 0%
17/04/17 16:51:20 INFO mapreduce.Job:  map 26% reduce 0%
17/04/17 16:51:22 INFO mapreduce.Job:  map 27% reduce 0%
17/04/17 16:51:28 INFO mapreduce.Job:  map 28% reduce 0%
17/04/17 16:51:30 INFO mapreduce.Job:  map 29% reduce 0%
17/04/17 16:51:36 INFO mapreduce.Job:  map 30% reduce 0%
17/04/17 16:51:39 INFO mapreduce.Job:  map 31% reduce 0%
17/04/17 16:51:45 INFO mapreduce.Job:  map 32% reduce 0%
17/04/17 16:51:47 INFO mapreduce.Job:  map 33% reduce 0%
17/04/17 16:51:51 INFO mapreduce.Job:  map 34% reduce 0%
17/04/17 16:51:55 INFO mapreduce.Job:  map 35% reduce 0%
17/04/17 16:51:58 INFO mapreduce.Job:  map 36% reduce 0%
17/04/17 16:52:02 INFO mapreduce.Job:  map 37% reduce 0%
17/04/17 16:52:06 INFO mapreduce.Job:  map 38% reduce 0%
17/04/17 16:52:11 INFO mapreduce.Job:  map 39% reduce 0%
17/04/17 16:52:15 INFO mapreduce.Job:  map 40% reduce 0%
17/04/17 16:52:16 INFO mapreduce.Job:  map 41% reduce 0%
17/04/17 16:52:22 INFO mapreduce.Job:  map 42% reduce 0%
17/04/17 16:52:24 INFO mapreduce.Job:  map 43% reduce 0%
17/04/17 16:52:30 INFO mapreduce.Job:  map 44% reduce 0%
17/04/17 16:52:32 INFO mapreduce.Job:  map 45% reduce 0%
17/04/17 16:52:39 INFO mapreduce.Job:  map 46% reduce 0%
17/04/17 16:52:41 INFO mapreduce.Job:  map 47% reduce 0%
17/04/17 16:52:44 INFO mapreduce.Job:  map 48% reduce 0%
17/04/17 16:52:50 INFO mapreduce.Job:  map 49% reduce 0%
17/04/17 16:52:51 INFO mapreduce.Job:  map 50% reduce 0%
17/04/17 16:52:57 INFO mapreduce.Job:  map 51% reduce 0%
17/04/17 16:52:59 INFO mapreduce.Job:  map 52% reduce 0%
17/04/17 16:53:05 INFO mapreduce.Job:  map 53% reduce 0%
17/04/17 16:53:07 INFO mapreduce.Job:  map 54% reduce 0%
17/04/17 16:53:11 INFO mapreduce.Job:  map 55% reduce 0%
17/04/17 16:53:16 INFO mapreduce.Job:  map 56% reduce 0%
17/04/17 16:53:18 INFO mapreduce.Job:  map 57% reduce 0%
17/04/17 16:53:24 INFO mapreduce.Job:  map 58% reduce 0%
17/04/17 16:53:27 INFO mapreduce.Job:  map 59% reduce 0%
17/04/17 16:53:32 INFO mapreduce.Job:  map 60% reduce 0%
17/04/17 16:53:35 INFO mapreduce.Job:  map 61% reduce 0%
17/04/17 16:53:39 INFO mapreduce.Job:  map 62% reduce 0%
17/04/17 16:53:42 INFO mapreduce.Job:  map 63% reduce 0%
17/04/17 16:53:45 INFO mapreduce.Job:  map 64% reduce 0%
17/04/17 16:53:51 INFO mapreduce.Job:  map 65% reduce 0%
17/04/17 16:53:55 INFO mapreduce.Job:  map 66% reduce 0%
17/04/17 16:53:57 INFO mapreduce.Job:  map 67% reduce 0%
17/04/17 16:54:01 INFO mapreduce.Job:  map 68% reduce 0%
17/04/17 16:54:05 INFO mapreduce.Job:  map 69% reduce 0%
17/04/17 16:54:09 INFO mapreduce.Job:  map 70% reduce 0%
17/04/17 16:54:12 INFO mapreduce.Job:  map 71% reduce 0%
17/04/17 16:54:17 INFO mapreduce.Job:  map 72% reduce 0%
17/04/17 16:54:22 INFO mapreduce.Job:  map 73% reduce 0%
17/04/17 16:54:25 INFO mapreduce.Job:  map 74% reduce 0%
17/04/17 16:54:30 INFO mapreduce.Job:  map 75% reduce 0%
17/04/17 16:54:31 INFO mapreduce.Job:  map 76% reduce 0%
17/04/17 16:54:35 INFO mapreduce.Job:  map 77% reduce 0%
17/04/17 16:54:40 INFO mapreduce.Job:  map 78% reduce 0%
17/04/17 16:54:43 INFO mapreduce.Job:  map 79% reduce 0%
17/04/17 16:54:48 INFO mapreduce.Job:  map 80% reduce 0%
17/04/17 16:54:51 INFO mapreduce.Job:  map 81% reduce 0%
17/04/17 16:54:56 INFO mapreduce.Job:  map 82% reduce 0%
17/04/17 16:54:59 INFO mapreduce.Job:  map 83% reduce 0%
17/04/17 16:55:03 INFO mapreduce.Job:  map 83% reduce 3%
17/04/17 16:55:07 INFO mapreduce.Job:  map 83% reduce 7%
17/04/17 16:55:09 INFO mapreduce.Job:  map 84% reduce 14%
17/04/17 16:55:12 INFO mapreduce.Job:  map 84% reduce 20%
17/04/17 16:55:15 INFO mapreduce.Job:  map 84% reduce 22%
17/04/17 16:55:17 INFO mapreduce.Job:  map 85% reduce 22%
17/04/17 16:55:18 INFO mapreduce.Job:  map 85% reduce 23%
17/04/17 16:55:21 INFO mapreduce.Job:  map 85% reduce 24%
17/04/17 16:55:23 INFO mapreduce.Job:  map 86% reduce 24%
17/04/17 16:55:29 INFO mapreduce.Job:  map 87% reduce 24%
17/04/17 16:55:32 INFO mapreduce.Job:  map 88% reduce 24%
17/04/17 16:55:38 INFO mapreduce.Job:  map 89% reduce 24%
17/04/17 16:55:39 INFO mapreduce.Job:  map 89% reduce 25%
17/04/17 16:55:45 INFO mapreduce.Job:  map 90% reduce 25%
17/04/17 16:55:51 INFO mapreduce.Job:  map 91% reduce 25%
17/04/17 16:55:57 INFO mapreduce.Job:  map 92% reduce 25%
17/04/17 16:56:00 INFO mapreduce.Job:  map 92% reduce 26%
17/04/17 16:56:03 INFO mapreduce.Job:  map 93% reduce 26%
17/04/17 16:56:08 INFO mapreduce.Job:  map 94% reduce 26%
17/04/17 16:56:14 INFO mapreduce.Job:  map 95% reduce 26%
17/04/17 16:56:20 INFO mapreduce.Job:  map 96% reduce 26%
17/04/17 16:56:21 INFO mapreduce.Job:  map 96% reduce 27%
17/04/17 16:56:28 INFO mapreduce.Job:  map 97% reduce 27%
17/04/17 16:56:34 INFO mapreduce.Job:  map 98% reduce 27%
17/04/17 16:56:40 INFO mapreduce.Job:  map 99% reduce 27%
17/04/17 16:56:43 INFO mapreduce.Job:  map 99% reduce 28%
17/04/17 16:56:45 INFO mapreduce.Job:  map 100% reduce 28%
17/04/17 16:56:47 INFO mapreduce.Job:  map 100% reduce 30%
17/04/17 16:56:49 INFO mapreduce.Job:  map 100% reduce 53%
17/04/17 16:56:50 INFO mapreduce.Job:  map 100% reduce 57%
17/04/17 16:56:52 INFO mapreduce.Job:  map 100% reduce 61%
17/04/17 16:56:53 INFO mapreduce.Job:  map 100% reduce 65%
17/04/17 16:56:55 INFO mapreduce.Job:  map 100% reduce 70%
17/04/17 16:56:56 INFO mapreduce.Job:  map 100% reduce 72%
17/04/17 16:56:58 INFO mapreduce.Job:  map 100% reduce 77%
17/04/17 16:56:59 INFO mapreduce.Job:  map 100% reduce 79%
17/04/17 16:57:01 INFO mapreduce.Job:  map 100% reduce 85%
17/04/17 16:57:02 INFO mapreduce.Job:  map 100% reduce 93%
17/04/17 16:57:03 INFO mapreduce.Job:  map 100% reduce 94%
17/04/17 16:57:05 INFO mapreduce.Job:  map 100% reduce 96%
17/04/17 16:57:08 INFO mapreduce.Job:  map 100% reduce 97%
17/04/17 16:57:11 INFO mapreduce.Job:  map 100% reduce 99%
17/04/17 16:57:14 INFO mapreduce.Job:  map 100% reduce 100%
17/04/17 16:57:14 INFO mapreduce.Job: Job job_1492459820743_0005 completed successfully
17/04/17 16:57:14 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=2908242405
                FILE: Number of bytes written=5801250620
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553659976
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=1194
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=12
        Job Counters
                Launched map tasks=392
                Launched reduce tasks=6
                Data-local map tasks=392
                Total time spent by all maps in occupied slots (ms)=2881135
                Total time spent by all reduces in occupied slots (ms)=662750
                Total time spent by all map tasks (ms)=2881135
                Total time spent by all reduce tasks (ms)=662750
                Total vcore-seconds taken by all map tasks=2881135
                Total vcore-seconds taken by all reduce tasks=662750
                Total megabyte-seconds taken by all map tasks=2950282240
                Total megabyte-seconds taken by all reduce tasks=678656000
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2843160699
                Input split bytes=59976
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2843160699
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =2352
                Failed Shuffles=0
                Merged Map outputs=2352
                GC time elapsed (ms)=35943
                CPU time spent (ms)=1433780
                Physical memory (bytes) snapshot=186126344192
                Virtual memory (bytes) snapshot=627387363328
                Total committed heap usage (bytes)=223297929216
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
17/04/17 16:57:14 INFO terasort.TeraSort: done
[neymar@ip-172-31-38-240 ec2-user]$
