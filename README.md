# jstackmem
Java stack memory calculator


用来统计 java 线程的内存占用大小

原理：统计 /proc/PID/smaps 文件，保存 Pss 那一列和对应的 LWP_ID 。然后通过 jstack 找到 LWP_ID 和线程名的对应关系。最后做统计。

