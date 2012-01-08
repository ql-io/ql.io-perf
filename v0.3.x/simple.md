# No Projections

select * from twitter.search where q = "ql.io";

## C=100

    ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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

    Document Path:          /q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        5924 bytes

    Concurrency Level:      100
    Time taken for tests:   49.189 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2032.98 [#/sec] (mean)
    Time per request:       49.189 [ms] (mean)
    Time per request:       0.492 [ms] (mean, across all concurrent requests)
    Transfer rate:          12201.85 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       4
    Processing:     5   49  48.2     32     528
    Waiting:        5   48  48.1     32     528
    Total:          5   49  48.2     32     528

    Percentage of the requests served within a certain time (ms)
      50%     32
      66%     45
      75%     57
      80%     68
      90%    108
      95%    150
      98%    204
      99%    243
     100%    528 (longest request)

## C=200

    ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"


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

    Document Path:          /q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        5924 bytes

    Concurrency Level:      200
    Time taken for tests:   48.576 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2058.63 [#/sec] (mean)
    Time per request:       97.152 [ms] (mean)
    Time per request:       0.486 [ms] (mean, across all concurrent requests)
    Transfer rate:          12355.79 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.2      0       7
    Processing:     5   97 135.2     42    1119
    Waiting:        5   96 135.1     42    1119
    Total:          5   97 135.2     43    1119

    Percentage of the requests served within a certain time (ms)
      50%     43
      66%     72
      75%    103
      80%    131
      90%    259
      95%    393
      98%    587
      99%    681
     100%   1119 (longest request)

## C=300

    ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"


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

    Document Path:          /q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        5924 bytes

    Concurrency Level:      300
    Time taken for tests:   49.184 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2033.17 [#/sec] (mean)
    Time per request:       147.553 [ms] (mean)
    Time per request:       0.492 [ms] (mean, across all concurrent requests)
    Transfer rate:          12202.97 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.5      0      13
    Processing:     5  147 228.2     56    1915
    Waiting:        5  146 228.2     55    1915
    Total:          5  147 228.2     56    1915

    Percentage of the requests served within a certain time (ms)
      50%     56
      66%    114
      75%    177
      80%    220
      90%    344
      95%    552
      98%   1053
      99%   1270
     100%   1915 (longest request)

## C=400

    ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"


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

    Document Path:          /q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        5924 bytes

    Concurrency Level:      400
    Time taken for tests:   50.198 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    1992.10 [#/sec] (mean)
    Time per request:       200.793 [ms] (mean)
    Time per request:       0.502 [ms] (mean, across all concurrent requests)
    Transfer rate:          11956.48 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.8      0      18
    Processing:     5  198 365.1     52    2234
    Waiting:        5  197 365.1     51    2234
    Total:          5  198 365.1     52    2235

    Percentage of the requests served within a certain time (ms)
      50%     52
      66%    106
      75%    176
      80%    239
      90%    512
      95%   1085
      98%   1646
      99%   1807
     100%   2235 (longest request)

## C=500

    ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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

    Document Path:          /q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        5924 bytes

    Concurrency Level:      500
    Time taken for tests:   49.909 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2003.66 [#/sec] (mean)
    Time per request:       249.543 [ms] (mean)
    Time per request:       0.499 [ms] (mean, across all concurrent requests)
    Transfer rate:          12025.88 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.9      0      18
    Processing:     5  246 331.0     97    2164
    Waiting:        5  245 330.9     96    2164
    Total:          5  246 331.0     97    2164

    Percentage of the requests served within a certain time (ms)
      50%     97
      66%    231
      75%    340
      80%    406
      90%    661
      95%    989
      98%   1364
      99%   1536
     100%   2164 (longest request)



