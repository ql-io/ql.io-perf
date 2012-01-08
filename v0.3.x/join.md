# Joins

    select ItemID, ViewItemURLForNaturalSearch, Location from details where itemId in
        (select itemId from finditems where keywords='mini cooper');

# C=100

    ab -c 100 -k -n 100000 -g c100.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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

## C=200

    ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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

## C=300

    ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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

## C=400

    ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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

    ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000/q?s=select%20ItemID%2C%20ViewItemURLForNaturalSearch%2C%20Location%20from%20details%20where%20itemId%20in%20%0A%20%20%20%20(select%20itemId%20from%20finditems%20where%20keywords%3D'mini%20cooper')%3B"

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

