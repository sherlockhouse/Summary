NOW()
===

NOW 函数返回当前的日期和时间。MySQL 语法：

```
SELECT NOW() FROM table_name
```

注：对于 Sql Server 数据库，使用 getdate() 函数来获得当前的日期时间。

### 示例

```
mysql> SELECT * FROM orders;
+----+--------+-----------+
| id | number | id_people |
+----+--------+-----------+
|  1 |    100 |         3 |
|  2 |    200 |         3 |
|  3 |    300 |         1 |
|  4 |    400 |         1 |
|  5 |    500 |         9 |
+----+--------+-----------+
5 rows in set (0.00 sec)

mysql> SELECT number, NOW() as time FROM orders;
+--------+---------------------+
| number | time                |
+--------+---------------------+
|    100 | 2015-09-12 18:39:57 |
|    200 | 2015-09-12 18:39:57 |
|    300 | 2015-09-12 18:39:57 |
|    400 | 2015-09-12 18:39:57 |
|    500 | 2015-09-12 18:39:57 |
+--------+---------------------+
5 rows in set (0.00 sec)
```
