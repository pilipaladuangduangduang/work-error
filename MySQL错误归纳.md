# MySQL错误归纳

标签（空格分隔）： 工作错误

---

## 在该笔记中记录工作开发过程中遇到的MySQL错误和解决方案：

### 主键重复错误

> MySQLIntegrityConstraintViolationException: <font color="FF2D2D">Duplicate entry</font>，表示表中有主键重复了；

### 日期时间类型转换时间戳错误
> java.sql.SQLException : Value '0000-00-00 00:00:00' can not be represented as java.sql.<font color="FF2D2D">Timestamp</font>，解决办法请参照这个链接地址：http://blog.sina.com.cn/s/blog_5fbb09180100u6xb.html；

### 由于MySQL使用utf8字符集不支持表情符号

 > 往数据库插入数据中包含表情符号或其他utf8不支持的特殊符号时会报这个错误：Incorrect string value: '\xF0\x9F\x92\x96\...' for column 'brief'

 > 做查询的时候，当查询条件参数中也包含特殊字符或表情字符，出现这个错误：Illegal mix of collations (utf8_general_ci,IMPLICIT) and (utf8mb4_general_ci,COERCIBLE) for operation '='
 
 > 以上两种错误的解决办法：将数据库的字符集改成<font color="FF2D2D">utf8mb4</font>。
 
### MySQL中查询关键字错误

 > <font color="FF2D2D">order</font>是MySQL中的关键字，做查询该字段的时候如果不通过``符号包裹或者表别名.order来查询就会报错。
 
  
