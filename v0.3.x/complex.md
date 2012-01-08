# myapi

    prodid = select ProductID[0].Value from eBay.FindProducts where
        QueryKeywords = 'macbook pro';
    details = select * from eBay.ProductDetails where
        ProductID in ('{prodid}') and ProductType = 'Reference';
    reviews = select * from eBay.ProductReviews where
        ProductID in ('{prodid}') and ProductType = 'Reference';

    return select d.ProductID[0].Value as id, d.Title as title,
        d.ReviewCount as reviewCount, r.ReviewDetails.AverageRating as rating
        from details as d, reviews as r
        where d.ProductID[0].Value = r.ProductID.Value
        via route '/myapi' using method get;

## C=100

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

## C=200

    ab -c 200 -k -n 100000 -g c200.dat "ql-2:3000/myapi"

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

## C=300

    ab -c 300 -k -n 100000 -g c300.dat "ql-2:3000/myapi"

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

## C=400

    ab -c 400 -k -n 100000 -g c400.dat "ql-2:3000/myapi"

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

## C=500

    ab -c 500 -k -n 100000 -g c500.dat "ql-2:3000/myapi"

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

