# JUnit错误归纳

标签（空格分隔）： 工作错误

---

## 在该笔记中记录工作开发过程中遇到的JUnit错误和解决方案：

### JUnit中测试方法不允许包含参数

> 今天在写JUnit单元测试的时候，不小心在测试方法中加了参数（TestNG写多了的后遗
症），然后运行JUnit就一直报错：junit.framework.AssertionFailedError: <font color="FF2D2D">No tests found in</font> com.xxx，后来才发现：在JUnit规范中<font color="FF2D2D">测试方法是不能包含参数</font>的！





