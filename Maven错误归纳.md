# Maven错误归纳

标签（空格分隔）： 工作错误

---

## 在该笔记中记录工作开发过程中遇到的Maven错误和解决方案：

### Maven和JDK版本不匹配

> 当JDK版本过低（比如1.6），Maven版本过高（比如3.2.1），在执行mvn clean install时，就会出抛出
java.lang.UnsupportedClassVersionError，解决办法就是：<font color="FF2D2D">升级JDK版本或者降低Maven版本</font>。

### Maven中compiler插件中遇到switch语法错误，编译失败

``` pom.xml
<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-compiler-plugin</artifactId>
	<version>${maven.compiler.plugin.version}</version>
	<configuration>
	    <!-- 1.6中switch语法是不支持String类型的，需要改成1.7及以上 -->
		<source>1.6</source>
		<target>1.6</target>
		<encoding>${project.build.sourceEncoding}</encoding>
	</configuration>
</plugin>
``` 


