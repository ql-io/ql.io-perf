# Request without project

select * from twitter.search where q = "ql.io";

## C 100

~/stack/ql.io-perf/v0.3.x/all> ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%
20%3D%20%22ql.io%22%3B"
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

## C 200

~/stack/ql.io-perf/v0.3.x/all> ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%
20%3D%20%22ql.io%22%3B"
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

## C 300

ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%
20%3D%20%22ql.io%22%3B"
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

## C 400


~/stack/ql.io-perf/v0.3.x/all> ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%
20%3D%20%22ql.io%22%3B"
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

## C 500

ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%
20%3D%20%22ql.io%22%3B"
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


# Request w Projections

## C 100

~/stack/ql.io-perf/v0.3.x/one> ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000/q?
s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20t
ext%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"
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


## C 200

~/stack/ql.io-perf/v0.3.x/one> ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000/q?
s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20t
ext%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"
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

## C 300

~/stack/ql.io-perf/v0.3.x/one> ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000/q?
s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20t
ext%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"
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

## C 400

~/stack/ql.io-perf/v0.3.x/one> ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000/q?
s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20t
ext%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"
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


## C 500

~/stack/ql.io-perf/v0.3.x/one> ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000/q?
s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20t
ext%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"
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

# Joins

# C 100

stack/ql.io-perf/v0.3.x/join> ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSear
ch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%
3D'mini%20cooper')%3B"
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

Document Path:          /q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B
Document Length:        1377 bytes

Concurrency Level:      100
Time taken for tests:   115.781 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      164800000 bytes
HTML transferred:       137700000 bytes
Requests per second:    863.70 [#/sec] (mean)
Time per request:       115.781 [ms] (mean)
Time per request:       1.158 [ms] (mean, across all concurrent requests)
Transfer rate:          1390.02 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.1      0       3
Processing:    12  115 110.8     82    2186
Waiting:       12  115 110.8     82    2186
Total:         12  116 110.8     83    2187

Percentage of the requests served within a certain time (ms)
  50%     83
  66%    107
  75%    128
  80%    145
  90%    222
  95%    360
  98%    489
  99%    552
 100%   2187 (longest request)

## C 200

ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSear
ch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%
3D'mini%20cooper')%3B"
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

Document Path:          /q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B
Document Length:        1377 bytes

Concurrency Level:      200
Time taken for tests:   116.018 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      164800000 bytes
HTML transferred:       137700000 bytes
Requests per second:    861.93 [#/sec] (mean)
Time per request:       232.037 [ms] (mean)
Time per request:       1.160 [ms] (mean, across all concurrent requests)
Transfer rate:          1387.17 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.2      0       7
Processing:    12  230 407.9     86    2508
Waiting:       12  230 407.9     86    2508
Total:         12  230 407.9     86    2508

Percentage of the requests served within a certain time (ms)
  50%     86
  66%    116
  75%    146
  80%    176
  90%    699
  95%   1300
  98%   1772
  99%   1936
 100%   2508 (longest request)

## C 300

ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%
2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'min
i%20cooper')%3B"
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

Document Path:          /q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B
Document Length:        1377 bytes

Concurrency Level:      300
Time taken for tests:   117.167 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      164800000 bytes
HTML transferred:       137700000 bytes
Requests per second:    853.48 [#/sec] (mean)
Time per request:       351.502 [ms] (mean)
Time per request:       1.172 [ms] (mean, across all concurrent requests)
Transfer rate:          1373.57 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.5      0      13
Processing:    12  347 587.7     94    3402
Waiting:       12  347 587.8     94    3402
Total:         12  347 587.8     94    3402

Percentage of the requests served within a certain time (ms)
  50%     94
  66%    135
  75%    194
  80%    394
  90%   1196
  95%   1715
  98%   2411
  99%   2666
 100%   3402 (longest request)

## C 400

ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%
2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'min
i%20cooper')%3B"
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

Document Path:          /q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B
Document Length:        1377 bytes

Concurrency Level:      400
Time taken for tests:   117.238 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      164800000 bytes
HTML transferred:       137700000 bytes
Requests per second:    852.97 [#/sec] (mean)
Time per request:       468.950 [ms] (mean)
Time per request:       1.172 [ms] (mean, across all concurrent requests)
Transfer rate:          1372.75 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.8      0      18
Processing:    12  464 860.9     98    4533
Waiting:       12  464 861.0     98    4533
Total:         12  464 860.9     98    4534

Percentage of the requests served within a certain time (ms)
  50%     98
  66%    147
  75%    260
  80%    561
  90%   1624
  95%   2557
  98%   3565
  99%   3878
 100%   4534 (longest request)

## C 500

ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%
2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'min
i%20cooper')%3B"
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

Document Path:          /q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B
Document Length:        1377 bytes

Concurrency Level:      500
Time taken for tests:   118.831 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      164800000 bytes
HTML transferred:       137700000 bytes
Requests per second:    841.53 [#/sec] (mean)
Time per request:       594.156 [ms] (mean)
Time per request:       1.188 [ms] (mean, across all concurrent requests)
Transfer rate:          1354.34 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   1.1      0      22
Processing:    12  585 852.1    119    3991
Waiting:       12  585 852.1    119    3991
Total:         12  585 852.1    119    3991

Percentage of the requests served within a certain time (ms)
  50%    119
  66%    392
  75%    901
  80%   1071
  90%   1921
  95%   2535
  98%   3346
  99%   3561
 100%   3991 (longest request)


# myapi

## C 100

~/stack/ql.io-perf/v0.3.x/script> ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000
/myapi"
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

## C 200

~/stack/ql.io-perf/v0.3.x/script> ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000
/myapi"
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
Time taken for tests:   465.370 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      131200000 bytes
HTML transferred:       60000000 bytes
Requests per second:    214.88 [#/sec] (mean)
Time per request:       930.740 [ms] (mean)
Time per request:       4.654 [ms] (mean, across all concurrent requests)
Transfer rate:          275.32 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.2      0       7
Processing:    30  918 2471.1    197   15711
Waiting:       30  918 2471.0    197   15711
Total:         30  919 2471.1    197   15712

Percentage of the requests served within a certain time (ms)
  50%    197
  66%    310
  75%    424
  80%    527
  90%   1099
  95%   8315
  98%  11462
  99%  12088
 100%  15712 (longest request)

## C 300

~/stack/ql.io-perf/v0.3.x/script> ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000
/myapi"
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

Concurrency Level:      300
Time taken for tests:   479.999 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      131200000 bytes
HTML transferred:       60000000 bytes
Requests per second:    208.33 [#/sec] (mean)
Time per request:       1439.998 [ms] (mean)
Time per request:       4.800 [ms] (mean, across all concurrent requests)
Transfer rate:          266.93 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    7 144.3      0    3010
Processing:    29 1419 2797.4    223   16039
Waiting:       29 1419 2797.4    223   16039
Total:         30 1426 2805.6    223   16039

Percentage of the requests served within a certain time (ms)
  50%    223
  66%    397
  75%    655
  80%   1252
  90%   5363
  95%   8262
  98%  11310
  99%  12238
 100%  16039 (longest request)

## C 400


~/stack/ql.io-perf/v0.3.x/script> ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000
/myapi"
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

Concurrency Level:      400
Time taken for tests:   513.985 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      131200000 bytes
HTML transferred:       60000000 bytes
Requests per second:    194.56 [#/sec] (mean)
Time per request:       2055.940 [ms] (mean)
Time per request:       5.140 [ms] (mean, across all concurrent requests)
Transfer rate:          249.28 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    5 136.1      0    9012
Processing:    29 2029 3600.8    264   25194
Waiting:       29 2029 3600.8    263   25194
Total:         30 2034 3605.7    264   25200

Percentage of the requests served within a certain time (ms)
  50%    264
  66%    527
  75%   1425
  80%   4286
  90%   7248
  95%  10980
  98%  13816
  99%  15042
 100%  25200 (longest request)

## C 500

~/stack/ql.io-perf/v0.3.x/script> ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000
/myapi"
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

Concurrency Level:      500
Time taken for tests:   520.375 seconds
Complete requests:      100000
Failed requests:        0
Write errors:           0
Keep-Alive requests:    0
Total transferred:      131200000 bytes
HTML transferred:       60000000 bytes
Requests per second:    192.17 [#/sec] (mean)
Time per request:       2601.874 [ms] (mean)
Time per request:       5.204 [ms] (mean, across all concurrent requests)
Transfer rate:          246.22 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   1.0      0      20
Processing:    29 2566 4183.6    296   23649
Waiting:       29 2566 4183.5    296   23649
Total:         30 2567 4183.6    296   23649

Percentage of the requests served within a certain time (ms)
  50%    296
  66%    678
  75%   3851
  80%   6445
  90%   9275
  95%  11799
  98%  14281
  99%  15755
 100%  23649 (longest request)

