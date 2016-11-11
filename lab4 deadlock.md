# lab4 deadlock

1. 死锁停在第几次的截图

   ![window.jpg](http://upload-images.jianshu.io/upload_images/3250499-36d5199b30306a37.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

2. 产生死锁的4个必要条件

   1. 资源互斥
   2. 持有锁并且等待
   3. 非抢占式调度
   4. 循环等待

3. 对上述程序产生死锁的解释

   上述的程序种包含两个进程，A进程和B进程，而在程序运行的时候设置count的值使得AB进程轮流占用资源，这时候就会出现资源调度，调度到的进程就会占用资源且运行，当调度到下一进程时资源仍被上个进程所占用，死锁产生的4个条件已经具备，这时候调度就会出现阻塞，进而产生死锁。