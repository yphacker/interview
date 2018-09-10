### 用SQL实现组内前几名的输出

```sql
selects  type, variety, price 
from fruits
where (
   select count(*) from fruits as f
   where f.type = fruits.type and f.price < fruits.price
) <= 1;
```
> 参考阅读
    - [如何用SQL实现组内前几名的输出](https://www.cnblogs.com/deng-cc/p/6363091.html)