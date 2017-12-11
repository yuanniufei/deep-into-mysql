# DEEP IN MySQL

## DML 语句

#### group by 之后可以一起显示总的 (with rollup)

```sql
select deptno,count(1) from emp group by deptno with rollup;

+---------------+----------+
| deptno        | COUNT(1) |
+---------------+----------+
| 2             | 81       |
| 4             | 34       |
| 7             | 23       |
| <null>        | 148      |
+---------------+----------+
```

## DCL 语句





