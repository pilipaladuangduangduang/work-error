# XML错误归纳

标签（空格分隔）： 工作错误

---

## 在该笔记中记录工作开发过程中遇到的XML错误和解决方案：


### XML编码问题

> <font color="FF2D2D">Invalid byte 1 of 1-byte UTF-8 sequence.</font> 当遇到这个错误的时候，首先检查XML文件的编码类型是否是Utf-8，如果不是Utf-8就讲编码格式改成Utf-8；如果是Utf-8那么就是XML中的中文有问题，删除注释中的中文。






