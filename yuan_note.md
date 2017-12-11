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

# 大纲

## 基础

- SQL基础
    - DDL
    - DML
    - DCL
- SQL数据类型
- 运算符
- 常用函数


SQL是结构化查询语言(Structure Query Language), 在使用之前提两个问题：

1. 什么是关系型数据库?
    关系型数据库，是指采用了关系模型来组织数据的数据库，就是二维表格模型，而一个关系型数据库就是由二维表及其之间的联系所组成的一个数据组织，关系型数据库的最大特点就是事务的一致性
    
2. 什么是NOSQL?
    NoSQL: Not only sql, 指代那些非关系型的，分布式的，且一般不保证遵循ACID原则的数据存储系统，可分为键值型(redis)，列存储(Cassandra, HBase)，文档型(MongoDb)，图形(InfoGrid)

3. RDBMS vs. NoSQL?

SQL基础，问题：

1. DDL, DML, DCL 分别表示什么？相关语句都有哪些？

    DDL:（Data Definition Language）数据库定义语言  CREATE, ALTER, DROP, TRUNCATE, COMMENT, RENAME
    DML: (Data Manipulation Language）数据操纵语言 SELECT, INSERT, UPDATE, DELETE, MERGE, CALL, EXPLAIN PLAN, LOCK TABLE
    DCL: Data Control Language）数据库控制语言 GRANT 授权, REVOKE 取消授权

2. 如何查看帮助？
     ? contents 

数据类型和运算符问题：

1. mysql都支持哪些数据类型?
    大致分为整形，浮点型，定点数，字符型，二进制，日期时间。

2. 如何选择合适的数据类型用较小的存储代价换来较高的数据库性能？
    根据具体的业务类型，并考虑以后业务的增长，合理选择数据类型及大小。









