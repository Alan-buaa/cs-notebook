# lsof

https://www.jianshu.com/p/a3aa6b01b2e1

lsof -n | awk '{print $2}' |  sort | uniq -c | sort -nr | more

当前系统各个进程产生了多少句柄 