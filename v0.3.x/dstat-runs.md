
## w=12



## w=96

    ~> ab -c 200 -k -n 100000 "ql-2:3000/myapi"
    This is ApacheBench, Version 2.3 <$Revision: 655654 $>
    Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
    Licensed to The Apache Software Foundation, http://www.apache.org/

    Benchmarking ql-2 (be patient)
    Completed 10000 requests
    Completed 20000 requests
    Completed 30000 requests
    Completed 40000 requests
    Completed 50000 requests
    Completed 60000 requests
    Completed 70000 requests
    Completed 80000 requests
    Completed 90000 requests
    Completed 100000 requests
    Finished 100000 requests


    Server Software:        ql.io/node.js
    Server Hostname:        ql-2
    Server Port:            3000

    Document Path:          /myapi
    Document Length:        600 bytes

    Concurrency Level:      200
    Time taken for tests:   279.391 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    357.92 [#/sec] (mean)
    Time per request:       558.783 [ms] (mean)
    Time per request:       2.794 [ms] (mean, across all concurrent requests)
    Transfer rate:          458.59 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.2      0      15
    Processing:    31  558 399.0    462    6509
    Waiting:       31  557 398.8    461    6509
    Total:         31  558 399.0    462    6515

    Percentage of the requests served within a certain time (ms)
      50%    462
      66%    588
      75%    704
      80%    784
      90%   1039
      95%   1311
      98%   1695
      99%   2016
     100%   6515 (longest request)