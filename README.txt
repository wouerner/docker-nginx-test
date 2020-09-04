docker-compose up --scale nginx=4
ab -n 500000 -c 1000 http://localhost:80/
/usr/bin/time -v ab -n 500000 -c 15000 http://localhost:80/



i5 7200u   

Command being timed: "ab -n 500000 -c 15000 http://localhost:80/"
        User time (seconds): 9.22
        System time (seconds): 1147.90
        Percent of CPU this job got: 94%
        Elapsed (wall clock) time (h:mm:ss or m:ss): 20:27.34
        Average shared text size (kbytes): 0
        Average unshared data size (kbytes): 0
        Average stack size (kbytes): 0
        Average total size (kbytes): 0
        Maximum resident set size (kbytes): 220048
        Average resident set size (kbytes): 0
        Major (requiring I/O) page faults: 0
        Minor (reclaiming a frame) page faults: 57739
        Voluntary context switches: 379
        Involuntary context switches: 219038
        Swaps: 0
        File system inputs: 0
        File system outputs: 0
        Socket messages sent: 0
        Socket messages received: 0
        Signals delivered: 0
        Page size (bytes): 4096
        Exit status: 0




AMD Ryzen 7 3800X 8-Core Processor

 Command being timed: "ab -n 500000 -c 15000 http://localhost:80/"
        User time (seconds): 2.24
        System time (seconds): 537.61
        Percent of CPU this job got: 99%
        Elapsed (wall clock) time (h:mm:ss or m:ss): 9:01.25
        Average shared text size (kbytes): 0
        Average unshared data size (kbytes): 0
        Average stack size (kbytes): 0
        Average total size (kbytes): 0
        Maximum resident set size (kbytes): 220088
        Average resident set size (kbytes): 0
        Major (requiring I/O) page faults: 0
        Minor (reclaiming a frame) page faults: 57792
        Voluntary context switches: 3
        Involuntary context switches: 64258
        Swaps: 0
        File system inputs: 0
        File system outputs: 0
        Socket messages sent: 0
        Socket messages received: 0
        Signals delivered: 0
        Page size (bytes): 4096
        Exit status: 0
