Linux如何查看端口

1、lsof -i:端口号 用于查看某一端口的占用情况，比如查看8000端口使用情况，lsof -i:8000

2、netstat -tunlp |grep 端口号，用于查看指定的端口号的进程情况，如查看8000端口的情况，netstat -tunlp |grep 8000

> 参考阅读
- [linux查看端口占用情况](https://www.cnblogs.com/wangtao1993/p/6144183.html)