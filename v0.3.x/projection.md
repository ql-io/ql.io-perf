# Projection

    select id as id, from_user_name as user_name, text as text
      from twitter.search where q = "ql.io";

## C=100

    ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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

    Document Path:          /q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        952 bytes

    Concurrency Level:      100
    Time taken for tests:   47.387 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2110.30 [#/sec] (mean)
    Time per request:       47.387 [ms] (mean)
    Time per request:       0.474 [ms] (mean, across all concurrent requests)
    Transfer rate:          2419.43 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0      10
    Processing:     5   47  45.9     32     558
    Waiting:        5   47  45.9     32     558
    Total:          5   47  45.9     33     558

    Percentage of the requests served within a certain time (ms)
      50%     33
      66%     45
      75%     56
      80%     66
      90%     96
      95%    132
      98%    190
      99%    242
     100%    558 (longest request)


## C=200

    ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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

    Document Path:          /q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        952 bytes

    Concurrency Level:      200
    Time taken for tests:   49.009 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2040.43 [#/sec] (mean)
    Time per request:       98.019 [ms] (mean)
    Time per request:       0.490 [ms] (mean, across all concurrent requests)
    Transfer rate:          2339.32 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.2      0       7
    Processing:     5   97 133.3     42    1000
    Waiting:        5   97 133.3     42    1000
    Total:          5   97 133.3     42    1000

    Percentage of the requests served within a certain time (ms)
      50%     42
      66%     69
      75%    102
      80%    137
      90%    271
      95%    400
      98%    534
      99%    637
     100%   1000 (longest request)

## C=300

    ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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

    Document Path:          /q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        952 bytes

    Concurrency Level:      300
    Time taken for tests:   48.750 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2051.27 [#/sec] (mean)
    Time per request:       146.251 [ms] (mean)
    Time per request:       0.488 [ms] (mean, across all concurrent requests)
    Transfer rate:          2351.74 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.4      0      11
    Processing:     5  145 189.2     57    1342
    Waiting:        5  145 189.2     57    1342
    Total:          5  146 189.2     58    1342

    Percentage of the requests served within a certain time (ms)
      50%     58
      66%    116
      75%    194
      80%    247
      90%    413
      95%    559
      98%    737
      99%    889
     100%   1342 (longest request)

## C=400

    ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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

    Document Path:          /q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        952 bytes

    Concurrency Level:      400
    Time taken for tests:   49.477 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2021.16 [#/sec] (mean)
    Time per request:       197.907 [ms] (mean)
    Time per request:       0.495 [ms] (mean, across all concurrent requests)
    Transfer rate:          2317.22 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.7      0      15
    Processing:     5  196 284.0     67    1829
    Waiting:        5  196 283.9     66    1829
    Total:          5  196 283.9     67    1830

    Percentage of the requests served within a certain time (ms)
      50%     67
      66%    139
      75%    223
      80%    294
      90%    599
      95%    909
      98%   1114
      99%   1209
     100%   1830 (longest request)


## C=500

    ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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

    Document Path:          /q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B
    Document Length:        952 bytes

    Concurrency Level:      500
    Time taken for tests:   50.180 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    1992.81 [#/sec] (mean)
    Time per request:       250.902 [ms] (mean)
    Time per request:       0.502 [ms] (mean, across all concurrent requests)
    Transfer rate:          2284.72 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.9      0      18
    Processing:     5  247 400.0     82    3001
    Waiting:        5  247 400.0     82    3001
    Total:          5  248 400.0     83    3001

    Percentage of the requests served within a certain time (ms)
      50%     83
      66%    182
      75%    277
      80%    361
      90%    672
      95%   1070
      98%   1788
      99%   2084
     100%   3001 (longest request)

