# Workers

# Workers = 12, c = 100

    ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000/myapi"

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

    Concurrency Level:      100
    Time taken for tests:   519.390 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    192.53 [#/sec] (mean)
    Time per request:       519.390 [ms] (mean)
    Time per request:       5.194 [ms] (mean, across all concurrent requests)
    Transfer rate:          246.68 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       4
    Processing:    30  518 604.5    307    6227
    Waiting:       30  518 604.5    307    6227
    Total:         30  519 604.5    307    6227

    Percentage of the requests served within a certain time (ms)
      50%    307
      66%    490
      75%    644
      80%    763
      90%   1208
      95%   1724
      98%   2479
      99%   3042
     100%   6227 (longest request)

# Workers = 24, c = 100

    ab -c 100 -k -n 100000 ql-2:3000/myapi

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

    Concurrency Level:      100
    Time taken for tests:   328.133 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    304.75 [#/sec] (mean)
    Time per request:       328.133 [ms] (mean)
    Time per request:       3.281 [ms] (mean, across all concurrent requests)
    Transfer rate:          390.47 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       3
    Processing:    27  327 332.0    224    6312
    Waiting:       27  327 332.0    224    6312
    Total:         27  328 332.0    225    6312

    Percentage of the requests served within a certain time (ms)
      50%    225
      66%    318
      75%    398
      80%    462
      90%    680
      95%    929
      98%   1330
      99%   1672
     100%   6312 (longest request)

## Workers = 36, c = 100

    ab -c 100 -k -n 100000 ql-2:3000/myapi

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

    Concurrency Level:      100
    Time taken for tests:   293.418 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    340.81 [#/sec] (mean)
    Time per request:       293.418 [ms] (mean)
    Time per request:       2.934 [ms] (mean, across all concurrent requests)
    Transfer rate:          436.66 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       4
    Processing:    28  293 239.7    225    3131
    Waiting:       28  293 239.6    224    3131
    Total:         28  293 239.7    225    3131

    Percentage of the requests served within a certain time (ms)
      50%    225
      66%    303
      75%    364
      80%    411
      90%    563
      95%    740
      98%   1019
      99%   1234
     100%   3131 (longest request)

# Workers = 48, c = 100

    ab -c 100 -k -n 100000 ql-2:3000/myapi

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

    Concurrency Level:      100
    Time taken for tests:   277.233 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    360.71 [#/sec] (mean)
    Time per request:       277.233 [ms] (mean)
    Time per request:       2.772 [ms] (mean, across all concurrent requests)
    Transfer rate:          462.16 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       4
    Processing:    30  277 205.5    227    4215
    Waiting:       30  276 205.5    227    4215
    Total:         30  277 205.5    227    4215

    Percentage of the requests served within a certain time (ms)
      50%    227
      66%    291
      75%    346
      80%    386
      90%    510
      95%    648
      98%    862
      99%   1046
     100%   4215 (longest request)

# Workers = 60, c = 100

    ab -c 100 -k -n 100000 ql-2:3000/myapi

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

    Concurrency Level:      100
    Time taken for tests:   269.323 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    371.30 [#/sec] (mean)
    Time per request:       269.323 [ms] (mean)
    Time per request:       2.693 [ms] (mean, across all concurrent requests)
    Transfer rate:          475.73 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       3
    Processing:    37  269 184.5    227    4028
    Waiting:       36  269 184.5    226    4028
    Total:         37  269 184.6    227    4031

    Percentage of the requests served within a certain time (ms)
      50%    227
      66%    289
      75%    336
      80%    376
      90%    494
      95%    609
      98%    779
      99%    912
     100%   4031 (longest request)

# Workers = 72, c = 100

    ab -c 100 -k -n 100000 ql-2:3000/myapi

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

    Concurrency Level:      100
    Time taken for tests:   265.262 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    376.99 [#/sec] (mean)
    Time per request:       265.262 [ms] (mean)
    Time per request:       2.653 [ms] (mean, across all concurrent requests)
    Transfer rate:          483.01 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       4
    Processing:    31  265 175.3    208    3852
    Waiting:       31  264 175.2    208    3852
    Total:         31  265 175.3    209    3855

    Percentage of the requests served within a certain time (ms)
      50%    209
      66%    294
      75%    337
      80%    365
      90%    485
      95%    600
      98%    756
      99%    886
     100%   3855 (longest request)


# Workers = 84, c = 100

    ab -c 100 -k -n 100000 ql-2:3000/myapi

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

    Concurrency Level:      100
    Time taken for tests:   261.781 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    382.00 [#/sec] (mean)
    Time per request:       261.781 [ms] (mean)
    Time per request:       2.618 [ms] (mean, across all concurrent requests)
    Transfer rate:          489.44 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       3
    Processing:    29  261 171.7    192    4907
    Waiting:       29  261 171.6    191    4907
    Total:         29  262 171.7    192    4910

    Percentage of the requests served within a certain time (ms)
      50%    192
      66%    271
      75%    338
      80%    369
      90%    465
      95%    589
      98%    742
      99%    865
     100%   4910 (longest request)

## Workers = 92, c = 100

    ab -c 100 -k -n 100000 ql-2:3000/myapi

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

    Concurrency Level:      100
    Time taken for tests:   260.079 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    384.50 [#/sec] (mean)
    Time per request:       260.079 [ms] (mean)
    Time per request:       2.601 [ms] (mean, across all concurrent requests)
    Transfer rate:          492.64 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       4
    Processing:    31  260 168.8    195    5076
    Waiting:       31  259 168.7    194    5076
    Total:         31  260 168.8    195    5078

    Percentage of the requests served within a certain time (ms)
      50%    195
      66%    244
      75%    313
      80%    365
      90%    453
      95%    574
      98%    727
      99%    861
     100%   5078 (longest request)