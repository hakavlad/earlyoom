# oomstat

oomstat is a very simple tool that prints available
memory, free swap and memory pressure (PSI) information
every 100ms.

Example output with `tail /dev/zero` started in the
background is pasted below, more examples are available
in the text files in this directory.


```
$ ./oomstat

./oomstat 
[sudo] password for jakob: 
     | /proc/meminfo     | /proc/pressure/memory
Time | MemAvail SwapFree | some avg10 full avg10
   s |      MiB      MiB |    %     %    %     %
     -                   -                      
 [...]
 1.5 |    20251        0 |    0     6    0     3
 1.6 |    20148        0 |    0     6    0     3
 1.7 |    19927        0 |    0     6    0     3
 1.8 |    19700        0 |    0     6    0     3
 1.9 |    19474        0 |    0     6    0     3
 2.0 |    19251        0 |    0     6    0     3
 2.1 |    19019        0 |    0     6    0     3
 2.2 |    18794        0 |    0     6    0     3
 2.3 |    18564        0 |    0     6    0     3
 2.4 |    18333        0 |    0     6    0     3
 2.5 |    18100        0 |    0     6    0     3
 2.6 |    17871        0 |    0     6    0     3
 2.7 |    17638        0 |    0     6    0     3
 2.8 |    17407        0 |    0     6    0     3
 2.9 |    17172        0 |    0     6    0     3
 3.0 |    16945        0 |    0     6    0     3
 3.1 |    16715        0 |    0     6    0     3
 3.2 |    16482        0 |    0     6    0     3
 3.3 |    16249        0 |    0     6    0     3
 3.4 |    16016        0 |    0     6    0     3
 3.5 |    15783        0 |    0     5    0     3
 3.6 |    15556        0 |    0     5    0     3
 3.7 |    15318        0 |    0     5    0     3
 3.8 |    15086        0 |    0     5    0     3
 3.9 |    14852        0 |    0     5    0     3
 4.0 |    14619        0 |    0     5    0     3
 4.1 |    14382        0 |    0     5    0     3
 4.2 |    14148        0 |    0     5    0     3
 4.3 |    13913        0 |    0     5    0     3
 4.4 |    13679        0 |    0     5    0     3
 4.5 |    13444        0 |    0     5    0     3
 4.6 |    13212        0 |    0     5    0     3
 4.7 |    12974        0 |    0     5    0     3
 4.8 |    12743        0 |    0     5    0     3
 4.9 |    12503        0 |    0     5    0     3
 5.0 |    12267        0 |    0     5    0     3
 5.1 |    12038        0 |    0     5    0     3
 5.2 |    11800        0 |    0     5    0     3
 5.3 |    11564        0 |    0     5    0     3
 5.4 |    11337        0 |    0     5    0     3
 5.5 |    11102        0 |    0     4    0     2
 5.6 |    10868        0 |    0     4    0     2
 5.7 |    10631        0 |    0     4    0     2
 5.8 |    10397        0 |    0     4    0     2
 5.9 |    10160        0 |    0     4    0     2
 6.0 |     9925        0 |    0     4    0     2
 6.1 |     9690        0 |    0     4    0     2
 6.2 |     9457        0 |    0     4    0     2
 6.3 |     9223        0 |    0     4    0     2
 6.4 |     8991        0 |    0     4    0     2
 6.5 |     8751        0 |    0     4    0     2
 6.6 |     8515        0 |    0     4    0     2
 6.7 |     8281        0 |    0     4    0     2
 6.8 |     8045        0 |    0     4    0     2
 6.9 |     7806        0 |    0     4    0     2
 7.0 |     7572        0 |    0     4    0     2
 7.1 |     7336        0 |    0     4    0     2
 7.2 |     7105        0 |    0     4    0     2
 7.3 |     6866        0 |    0     4    0     2
 7.4 |     6631        0 |    0     4    0     2
 7.5 |     6396        0 |    0     3    0     2
 7.6 |     6160        0 |    0     3    0     2
 7.7 |     5921        0 |    0     3    0     2
 7.8 |     5689        0 |    0     3    0     2
 7.9 |     5452        0 |    0     3    0     2
 8.0 |     5219        0 |    0     3    0     2
 8.1 |     4983        0 |    0     3    0     2
 8.2 |     4748        0 |    0     3    0     2
 8.3 |     4513        0 |    0     3    0     2
 8.4 |     4278        0 |    0     3    0     2
 8.5 |     4038        0 |    0     3    0     2
 8.6 |     3805        0 |    0     3    0     2
 8.7 |     3570        0 |    0     3    0     2
 8.8 |     3338        0 |    0     3    0     2
 8.9 |     3103        0 |    0     3    0     2
 9.0 |     2868        0 |    0     3    0     2
 9.1 |     2637        0 |    0     3    0     2
 9.2 |     2405        0 |    0     3    0     2
 9.3 |     2167        0 |    0     3    0     2
 9.4 |     1935        0 |    0     3    0     2
 9.5 |     1701        0 |    0     2    0     1
 9.6 |     1467        0 |    0     2    0     1
 9.7 |     1231        0 |    0     2    0     1
 9.8 |      999        0 |    0     2    0     1
 9.9 |      767        0 |    0     2    0     1
10.0 |      532        0 |    0     2    0     1
10.1 |      313        0 |    0     2    0     1
10.2 |       91        0 |    5     2    3     1
10.3 |       52        0 |   61     2   43     1
10.4 |       29        0 |   55     2   39     1
10.5 |        0        0 |   64     2   46     1
10.6 |        0        0 |   95     2   75     1
10.7 |        0        0 |   98     2   85     1
11.3 |        0        0 |   99    12   91     9
13.2 |        0        0 |  100    28   91    24
14.3 |     2014        0 |   88    28   47    24
14.4 |     6915        0 |   18    28   10    24
14.5 |    12071        0 |    0    28    0    24
14.6 |    17071        0 |    0    28    0    24
14.7 |    20290        0 |    0    28    0    24
14.8 |    20283        0 |    0    28    0    24
14.9 |    20283        0 |    0    28    0    24
15.0 |    20283        0 |    0    28    0    24
15.1 |    20283        0 |    0    28    0    24
15.2 |    20283        0 |    0    28    0    24
15.3 |    20277        0 |    0    28    0    24
15.4 |    20267        0 |    0    28    0    24
15.5 |    20267        0 |    0    28    0    24
15.6 |    20266        0 |    0    30    0    26
15.7 |    20266        0 |    0    30    0    26
15.8 |    20267        0 |    0    30    0    26
15.9 |    20260        0 |    0    30    0    26
16.0 |    20261        0 |    0    30    0    26
16.1 |    20264        0 |    0    30    0    26
16.2 |    20265        0 |    0    30    0    26
16.3 |    20259        0 |    0    30    0    26
16.4 |    20262        0 |    0    30    0    26
```