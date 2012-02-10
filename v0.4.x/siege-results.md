Load test with siege 2.70
==========================

Setup
======
Server - 10.254.32.109 (see below for the configuration detials)
Client - ql.corp.ebay.com
Traffice server - ql-1.corp.ebay.com

The testing was performed with the command,

        siege -c<Conurrency> -r100 -d0 http://10.254.32.109:3000/q?s=select%20*%20from%20twitter.search%20where%21q%20%3D%20%22ql.io%22%3B

        where 'Concurrency' is 100, 200, 300, 400 and 500.

Corresponding results for the above set of runs.


ql.io 0.4 in node 0.6.10
========================
      Date & Time,  Trans,  Elap Time,  Data Trans,  Resp Time,  Trans Rate,  Throughput,  Concurrent,    OKAY,   Failed
2012-02-09 22:28:46,  10000,      12.49,         119,       0.12,      800.64,        9.53,       98.29,   10000,       0
2012-02-09 22:29:35,  20000,      24.36,         238,       0.22,      821.02,        9.77,      181.57,   20000,       0
2012-02-09 22:30:26,  30000,      36.63,         358,       0.32,      819.00,        9.77,      261.02,   30000,       0
2012-02-09 22:33:23,  40000,      49.04,         477,       0.39,      815.66,        9.73,      320.83,   40000,       0
2012-02-09 22:37:47,  50000,      60.49,         596,       0.51,      826.58,        9.85,      421.85,   50000,       0



ql.io 0.3 in node 0.4.12
========================
      Date & Time,  Trans,  Elap Time,  Data Trans,  Resp Time,  Trans Rate,  Throughput,  Concurrent,    OKAY,   Failed
2012-02-10 10:13:12,   9999,     130.46,         136,       0.14,       76.64,        1.04,       10.57,    9999,       1
2012-02-10 10:15:58,  19992,     142.90,         273,       0.28,      139.90,        1.91,       38.78,   19992,       8
2012-02-10 10:31:04,  29997,     155.93,         410,       0.35,      192.37,        2.63,       68.00,   29997,       3
2012-02-10 10:33:41,  39999,     127.36,         548,       0.47,      314.06,        4.30,      149.09,   39999,       1
2012-02-10 10:36:52,  49998,     129.50,         685,       0.60,      386.08,        5.29,      231.15,   49998,       2



Server machine configuration
=============================
width: 64 bits
    capabilities: vsyscall64 vsyscall32
  *-core
       description: Motherboard
       physical id: 0
     *-memory
          description: System memory
          physical id: 0
          size: 23GiB
     *-cpu:0
          product: Intel(R) Xeon(R) CPU           E5645  @ 2.40GHz
          vendor: Intel Corp.
          physical id: 1
          bus info: cpu@0
          width: 64 bits
     *-cpu:1
          product: Intel(R) Xeon(R) CPU           E5645  @ 2.40GHz
          vendor: Intel Corp.
          physical id: 2
          bus info: cpu@1
          width: 64 bits

Network RTT
===========
Server machine to ql-1 - rtt min/avg/max/mdev = 0.254/0.281/0.298/0.022 ms
Client to Server - rtt min/avg/max/mdev = 0.274/0.284/0.322/0.012 ms


