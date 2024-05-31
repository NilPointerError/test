**COUNT(*) COUNT(1) COUNT(列名)有什么区别？**

COUNT(*) 和 COUNT(1) 没有区别，计算的都是总行数，统计null值

count(列名)计算的是列的行数，不统计null值



数据库名、表名、列名 小写   （与关键词重复要用 `` 括起来）

函数名、关键词大写

windows不区分大小写  linux区分大小写

数据库名不能修改



**group by**

group by 子句中应该有select 中所有不包含聚合函数的字段（only_full_group模式，防止非聚合列分组产生歧义）

group by子句中会有select中没有的字段



**having**

使用having之前需要groupby分组，对聚合函数进行筛选（与where不同）

where可以先筛选后连接，having是先连接后筛选，效率显然比where低、

**子查询**

相关子查询、不相关子查询

EXISTS、NOT EXISTS   ANY、IN、ALL      



**事务**
drop、truncate等DDL语句不能回滚

delete 等DML语句可以回滚

truncate与delete区别？



sql_mode,"ONLY_FULL_GROUP_BY,STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_ENGINE_SUBSTITUTION"





