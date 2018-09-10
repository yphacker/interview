### linux查找目录下的所有文件中是否含有某个字符串

查找目录下的所有文件中是否含有某个字符串 
find .|xargs grep -ri "IBM" 
查找目录下的所有文件中是否含有某个字符串,并且只打印出文件名 
find .|xargs grep -ri "IBM" -l 

> 参考阅读
- [查找目录下的所有文件中是否含有某个字符串](http://blog.sina.com.cn/s/blog_691a84f301015khx.html)