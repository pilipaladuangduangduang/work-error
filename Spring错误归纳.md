# Spring错误归纳

标签（空格分隔）： 工作错误

---

## 在该笔记中记录工作开发过程中遇到的Spring错误和解决方案：

### SpringMVC返回HttpStatus 400 Bad Request

今天在做前后端传输数据的时候，发起请求总是返回400错误，经历一番搜索后发现是因为后端方法中的所需的参数前端没有提供对应name的数据就报错了，之后把后端方法中参数的<font color="FF2D2D">@RequestParam属性required设置为false</font>就OK了，具体错误如下：

``` 
HTTP Status 400 ———— The request sent by the client was syntactically incorrect ().
``` 




