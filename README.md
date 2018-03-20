# GCD
GCD由浅入深

1、基础语法

串行队列DISPATCH_QUEUE_SERIAL 、并发队列DISPATCH_QUEUE_CONCURRENT基本创建使用；

http://www.chuliangliang.com/2017/03/27/iOS-GCD-Grand-Central-Dispatch-1/

2、分组执行 与 分发

手动调动组、自动调动组、等待群组任务完成disaptch_group_wait

http://www.chuliangliang.com/2017/04/06/iOS-GCD-Grand-Central-Dispatch-2/

3、队列的挂起、恢复 ，栅栏

dispatch_suspend 与 dispatch_resume 成对出现;
dispatch_barrier_sync将自己的任务插入到队列的时候，需要等待自己的任务结束之后才会继续插入被写在它后面的任务，然后执行它们。
dispatch_barrier_async将自己的任务插入到队列之后，不会等待自己的任务结束，它会继续把后面的任务插入到队列，然后等待自己的任务结束后才执行后面任务

http://www.chuliangliang.com/2017/05/02/iOS-GCD-Grand-Central-Dispatch-3/
