### 统计nginx日志中访问次数前十个IP

```bash
awk '{print $1}' urlogfile | sort | uniq -c | sort -nr -k1 | head -n 10
awk '{print $1}' /usr/local/nginx/logs/localhost.access.log | sort | uniq -c | sort -nr -k1 | head -n 10
```

> 参考阅读
- [统计Apache或nginx日志里访问次数最多的前十个IP](http://www.07net01.com/2015/08/914079.html)