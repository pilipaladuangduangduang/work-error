# MyBatis错误归纳

标签（空格分隔）： 工作错误

---

## 在该笔记中记录工作开发过程中遇到的MyBatis错误和解决方案：

### 表中的列和插入的值匹配不上

> MyBatis中遇到<font color="FF2D2D">Column count doesn't match value count</font> at row 1 是因为列和值的个数不相等，这时候先检查列和值的逗号是否有漏写。

### MyBatis的配置文件不支持映射Class类型的字段

> org.apache.ibatis.builder.BuilderException: Error parsing Mapper XML. Cause: java.lang.IllegalStateException: <font color="FF2D2D">No typehandler found for property objClazz</font>




