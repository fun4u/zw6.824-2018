### MIT6.824-2018
this is zhangwei's MIT6.824 experiment practice

#### rework lab 2a:
##### 1. 事件驱动状态机
##### 2. 多线程pipeline
##### 3. 基于通信而不是基于锁的共享内存

* Test (2A): initial election ...
*  ... Passed --   3.1  3   30    0
* Test (2A): election after network failure ...
*  ... Passed --   4.5  3   68    0
* PASS
* ok      raft    7.647s

* Test (2B): basic agreement ...
*  ... Passed --   1.5  5   36    3
* Test (2B): agreement despite follower disconnection ...
*  ... Passed --   5.2  3   74    7
* Test (2B): no agreement if too many followers disconnect ...
*  ... Passed --   4.0  5  156    4
* Test (2B): concurrent Start()s ...
*  ... Passed --   0.8  3   10    6
* Test (2B): rejoin of partitioned leader ...
*  ... Passed --   7.3  3  128    4
* Test (2B): leader backs up quickly over incorrect follower logs ...
*  ... Passed --  49.2  5 2544  105
* Test (2B): RPC counts aren't too high ...
*   ... Passed --   2.8  3   30   12
* PASS
* ok      raft    70.933s

* Test (2C): basic persistence ...
*   ... Passed --   5.5  3   76    6
* Test (2C): more persistence ...
*   ... Passed --  20.0  5  732   16
* Test (2C): partitioned leader and one follower crash, leader restarts ...
*   ... Passed --   2.8  3   34    4
* Test (2C): Figure 8 ...
*   ... Passed --  37.9  5  936   16
* Test (2C): unreliable agreement ...
*   ... Passed --  13.6  5  336  246
* Test (2C): Figure 8 (unreliable) ...
*   ... Passed --  35.0  5 2220  911
* Test (2C): churn ...
*  ... Passed --  16.3  5  428  181
* Test (2C): unreliable churn ...
*  ... Passed --  16.4  5  500  122
* PASS
* ok      raft    147.469s
