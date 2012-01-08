
## Simple

### c = 100

    ab -c 100 -k -n 100000 "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   41.335 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2419.28 [#/sec] (mean)
    Time per request:       41.335 [ms] (mean)
    Time per request:       0.413 [ms] (mean, across all concurrent requests)
    Transfer rate:          14520.43 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0  13.4      0    3004
    Processing:     4   41  57.9     18    1193
    Waiting:        4   40  57.3     17    1193
    Total:          5   41  59.4     18    3036

    Percentage of the requests served within a certain time (ms)
      50%     18
      66%     41
      75%     56
      80%     66
      90%     97
      95%    132
      98%    219
      99%    289
     100%   3036 (longest request)

### c=200

    ab -c 200 -k -n 100000 "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   40.301 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2481.33 [#/sec] (mean)
    Time per request:       80.602 [ms] (mean)
    Time per request:       0.403 [ms] (mean, across all concurrent requests)
    Transfer rate:          14892.82 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0  28.5      0    3006
    Processing:     4   80  79.1     64     964
    Waiting:        4   78  78.3     62     963
    Total:          4   80  84.4     64    3235

    Percentage of the requests served within a certain time (ms)
      50%     64
      66%     91
      75%    111
      80%    125
      90%    168
      95%    221
      98%    318
      99%    383
     100%   3235 (longest request)

### c=300

    ab -c 300 -k -n 100000 "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   39.623 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2523.78 [#/sec] (mean)
    Time per request:       118.869 [ms] (mean)
    Time per request:       0.396 [ms] (mean, across all concurrent requests)
    Transfer rate:          15147.62 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    1  35.5      0    3004
    Processing:     4  118  98.7     97    1186
    Waiting:        4  115  97.6     94    1186
    Total:          5  119 105.5     97    3332

    Percentage of the requests served within a certain time (ms)
      50%     97
      66%    134
      75%    157
      80%    175
      90%    236
      95%    308
      98%    406
      99%    472
     100%   3332 (longest request)

### c-400

    ab -c 400 -k -n 100000 "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   39.586 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2526.13 [#/sec] (mean)
    Time per request:       158.345 [ms] (mean)
    Time per request:       0.396 [ms] (mean, across all concurrent requests)
    Transfer rate:          15161.70 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.6      0      14
    Processing:     5  158 124.2    132    1755
    Waiting:        4  154 123.0    129    1755
    Total:          5  158 124.2    132    1755

    Percentage of the requests served within a certain time (ms)
      50%    132
      66%    171
      75%    205
      80%    228
      90%    310
      95%    398
      98%    512
      99%    597
     100%   1755 (longest request)

### C=500

    ab -c 500 -k -n 100000 "ql-2:3000/q?s=select%20*%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   39.649 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      614600000 bytes
    HTML transferred:       592400000 bytes
    Requests per second:    2522.16 [#/sec] (mean)
    Time per request:       198.243 [ms] (mean)
    Time per request:       0.396 [ms] (mean, across all concurrent requests)
    Transfer rate:          15137.90 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0  25.1      0    3004
    Processing:     4  197 164.9    156    2025
    Waiting:        4  194 163.7    153    2025
    Total:          5  198 166.8    156    3226

    Percentage of the requests served within a certain time (ms)
      50%    156
      66%    209
      75%    248
      80%    278
      90%    388
      95%    512
      98%    685
      99%    836
     100%   3226 (longest request)


## Projections

### c = 100

    ab -c 100 -k -n 100000 "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   41.908 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2386.20 [#/sec] (mean)
    Time per request:       41.908 [ms] (mean)
    Time per request:       0.419 [ms] (mean, across all concurrent requests)
    Transfer rate:          2735.74 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       3
    Processing:     4   42  54.6     20    1058
    Waiting:        4   41  54.3     20    1058
    Total:          4   42  54.6     20    1059

    Percentage of the requests served within a certain time (ms)
      50%     20
      66%     44
      75%     59
      80%     69
      90%     99
      95%    131
      98%    200
      99%    275
     100%   1059 (longest request)

### c = 200

    ab -c 200 -k -n 100000 "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   40.890 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2445.59 [#/sec] (mean)
    Time per request:       81.780 [ms] (mean)
    Time per request:       0.409 [ms] (mean, across all concurrent requests)
    Transfer rate:          2803.83 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    1  39.2      0    3010
    Processing:     4   81  77.6     66    1185
    Waiting:        4   80  77.4     65    1125
    Total:          5   82  87.9     66    3559

    Percentage of the requests served within a certain time (ms)
      50%     66
      66%     93
      75%    115
      80%    128
      90%    170
      95%    218
      98%    313
      99%    376
     100%   3559 (longest request)

### c = 300

    ab -c 300 -k -n 100000 "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   40.581 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2464.19 [#/sec] (mean)
    Time per request:       121.744 [ms] (mean)
    Time per request:       0.406 [ms] (mean, across all concurrent requests)
    Transfer rate:          2825.15 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    4 104.1      0    3010
    Processing:     4  118  98.9     98    3788
    Waiting:        4  117  98.7     97    3788
    Total:          5  122 150.2     98    4233

    Percentage of the requests served within a certain time (ms)
      50%     98
      66%    135
      75%    157
      80%    174
      90%    234
      95%    307
      98%    406
      99%    477
     100%   4233 (longest request)

### c = 400

    ab -c 400 -k -n 100000 "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   40.355 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2477.98 [#/sec] (mean)
    Time per request:       161.422 [ms] (mean)
    Time per request:       0.404 [ms] (mean, across all concurrent requests)
    Transfer rate:          2840.96 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0  21.2      0    3003
    Processing:     4  161 122.4    136    1554
    Waiting:        4  160 122.2    135    1554
    Total:          5  161 124.3    136    3219

    Percentage of the requests served within a certain time (ms)
      50%    136
      66%    176
      75%    209
      80%    231
      90%    309
      95%    396
      98%    515
      99%    597
     100%   3219 (longest request)

### c = 500

    ab -c 500 -k -n 100000 "ql-2:3000/q?s=select%20id%20as%20id%2C%20from_user_name%20as%20user_name%2C%20text%20as%20text%0A%20%20from%20twitter.search%20where%20q%20%3D%20%22ql.io%22%3B"

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
    Time taken for tests:   39.953 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      117400000 bytes
    HTML transferred:       95200000 bytes
    Requests per second:    2502.91 [#/sec] (mean)
    Time per request:       199.767 [ms] (mean)
    Time per request:       0.400 [ms] (mean, across all concurrent requests)
    Transfer rate:          2869.55 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.9      0      18
    Processing:     4  199 178.5    159    2981
    Waiting:        4  198 178.3    158    2981
    Total:          5  199 178.5    159    2981

    Percentage of the requests served within a certain time (ms)
      50%    159
      66%    208
      75%    246
      80%    274
      90%    376
      95%    492
      98%    663
      99%    846
     100%   2981 (longest request)


## Join

### c = 100

    ab -c 100 -k -n 100000 "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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
    Document Length:        1466 bytes

    Concurrency Level:      100
    Time taken for tests:   101.776 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      173700000 bytes
    HTML transferred:       146600000 bytes
    Requests per second:    982.55 [#/sec] (mean)
    Time per request:       101.776 [ms] (mean)
    Time per request:       1.018 [ms] (mean, across all concurrent requests)
    Transfer rate:          1666.70 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.1      0       9
    Processing:    11  102  79.4     79    3164
    Waiting:       11  101  79.2     79    3164
    Total:         11  102  79.4     79    3167

    Percentage of the requests served within a certain time (ms)
      50%     79
      66%    112
      75%    131
      80%    145
      90%    195
      95%    247
      98%    330
      99%    389
     100%   3167 (longest request)

### c = 200

    ab -c 200 -k -n 100000 "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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
    Document Length:        1466 bytes

    Concurrency Level:      200
    Time taken for tests:   100.300 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      173700000 bytes
    HTML transferred:       146600000 bytes
    Requests per second:    997.00 [#/sec] (mean)
    Time per request:       200.601 [ms] (mean)
    Time per request:       1.003 [ms] (mean, across all concurrent requests)
    Transfer rate:          1691.21 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   9.5      0    3004
    Processing:    11  200 128.2    174    3751
    Waiting:       11  200 128.0    173    3751
    Total:         11  200 128.6    174    3757

    Percentage of the requests served within a certain time (ms)
      50%    174
      66%    224
      75%    257
      80%    281
      90%    358
      95%    439
      98%    550
      99%    637
     100%   3757 (longest request)


### c = 300

    ab -c 300 -k -n 100000 "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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
    Document Length:        1466 bytes

    Concurrency Level:      300
    Time taken for tests:   100.293 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      173700000 bytes
    HTML transferred:       146600000 bytes
    Requests per second:    997.08 [#/sec] (mean)
    Time per request:       300.880 [ms] (mean)
    Time per request:       1.003 [ms] (mean, across all concurrent requests)
    Transfer rate:          1691.33 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    1  57.0      0    3010
    Processing:    12  299 168.5    264    1730
    Waiting:       12  298 168.3    264    1730
    Total:         13  300 181.0    265    4247

    Percentage of the requests served within a certain time (ms)
      50%    265
      66%    329
      75%    378
      80%    412
      90%    516
      95%    622
      98%    760
      99%    864
     100%   4247 (longest request)

### c = 400

    ab -c 400 -k -n 100000 "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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
    Document Length:        1466 bytes

    Concurrency Level:      400
    Time taken for tests:   100.568 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      173700000 bytes
    HTML transferred:       146600000 bytes
    Requests per second:    994.35 [#/sec] (mean)
    Time per request:       402.272 [ms] (mean)
    Time per request:       1.006 [ms] (mean, across all concurrent requests)
    Transfer rate:          1686.71 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.7      0      32
    Processing:    12  401 221.9    354    2288
    Waiting:       12  400 221.6    353    2288
    Total:         13  402 221.9    354    2288

    Percentage of the requests served within a certain time (ms)
      50%    354
      66%    442
      75%    506
      80%    551
      90%    691
      95%    829
      98%   1006
      99%   1139
     100%   2288 (longest request)

### c = 500

    ab -c 500 -k -n 100000 "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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
    Document Length:        1466 bytes

    Concurrency Level:      500
    Time taken for tests:   110.338 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      173700000 bytes
    HTML transferred:       146600000 bytes
    Requests per second:    906.30 [#/sec] (mean)
    Time per request:       551.692 [ms] (mean)
    Time per request:       1.103 [ms] (mean, across all concurrent requests)
    Transfer rate:          1537.35 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    1  28.5      0    3008
    Processing:    12  550 720.2    439   13047
    Waiting:       12  549 720.1    438   13047
    Total:         13  551 721.7    439   13062

    Percentage of the requests served within a certain time (ms)
      50%    439
      66%    551
      75%    638
      80%    699
      90%    881
      95%   1076
      98%   1389
      99%   1808
     100%  13062 (longest request)

## Complex

### c = 100

    ~> ab -c 100 -k -n 100000 "ql-2:3000/myapi"
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
    Time taken for tests:   261.773 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    382.01 [#/sec] (mean)
    Time per request:       261.773 [ms] (mean)
    Time per request:       2.618 [ms] (mean, across all concurrent requests)
    Transfer rate:          489.45 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0  16.5      0    3004
    Processing:    36  261 162.8    195    2617
    Waiting:       36  261 162.6    195    2617
    Total:         36  262 164.3    196    4713

    Percentage of the requests served within a certain time (ms)
      50%    196
      66%    245
      75%    317
      80%    368
      90%    459
      95%    585
      98%    736
      99%    875
     100%   4713 (longest request)

### c = 200

    ab -c 200 -k -n 100000 "ql-2:3000/myapi"

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
    Time taken for tests:   281.292 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    355.50 [#/sec] (mean)
    Time per request:       562.584 [ms] (mean)
    Time per request:       2.813 [ms] (mean, across all concurrent requests)
    Transfer rate:          455.49 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.3      0       8
    Processing:    85  562 396.3    465    6572
    Waiting:       85  561 396.1    464    6572
    Total:         86  562 396.3    465    6576

    Percentage of the requests served within a certain time (ms)
      50%    465
      66%    597
      75%    715
      80%    797
      90%   1045
      95%   1310
      98%   1690
      99%   1983
     100%   6576 (longest request)

### c = 300

    ab -c 300 -k -n 100000 "ql-2:3000/myapi"

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
    Time taken for tests:   307.951 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    324.73 [#/sec] (mean)
    Time per request:       923.852 [ms] (mean)
    Time per request:       3.080 [ms] (mean, across all concurrent requests)
    Transfer rate:          416.06 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0  19.0      0    3004
    Processing:    77  922 777.6    698   11040
    Waiting:       77  921 777.4    697   11040
    Total:         77  922 777.9    699   11041

    Percentage of the requests served within a certain time (ms)
      50%    699
      66%    938
      75%   1138
      80%   1286
      90%   1811
      95%   2409
      98%   3241
      99%   3945
     100%  11041 (longest request)

### c = 400

    ab -c 400 -k -n 100000 "ql-2:3000/myapi"

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
    Time taken for tests:   335.948 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    297.66 [#/sec] (mean)
    Time per request:       1343.793 [ms] (mean)
    Time per request:       3.359 [ms] (mean, across all concurrent requests)
    Transfer rate:          381.38 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   0.8      0      16
    Processing:    46 1339 1339.9    906   16313
    Waiting:       46 1338 1339.6    904   16057
    Total:         46 1340 1340.0    906   16313

    Percentage of the requests served within a certain time (ms)
      50%    906
      66%   1284
      75%   1623
      80%   1892
      90%   2811
      95%   3909
      98%   5568
      99%   6934
     100%  16313 (longest request)

### c = 500

    ab -c 500 -k -n 100000 "ql-2:3000/myapi"

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
    Time taken for tests:   354.440 seconds
    Complete requests:      100000
    Failed requests:        0
    Write errors:           0
    Keep-Alive requests:    0
    Total transferred:      131200000 bytes
    HTML transferred:       60000000 bytes
    Requests per second:    282.14 [#/sec] (mean)
    Time per request:       1772.200 [ms] (mean)
    Time per request:       3.544 [ms] (mean, across all concurrent requests)
    Transfer rate:          361.49 [Kbytes/sec] received

    Connection Times (ms)
                  min  mean[+/-sd] median   max
    Connect:        0    0   1.0      0      20
    Processing:    98 1766 2612.7   1027   58755
    Waiting:       98 1764 2612.4   1027   58755
    Total:         98 1766 2612.8   1028   58755

    Percentage of the requests served within a certain time (ms)
      50%   1028
      66%   1504
      75%   1945
      80%   2300
      90%   3564
      95%   5223
      98%   9357
      99%  13374
     100%  58755 (longest request)
