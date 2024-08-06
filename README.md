# JavaSec
Java安全学习记录
Java 安全学习路线

# IDEA
IDEA安装

如何调试，如何下断电，如何远程调试

常见bug如何解决

# Maven
Maven安装配置

常见bug解决

镜像文件如何加速，用阿里云镜像

各种常见Maven插件

多模块项目是什么

了解Gradle

# Java Web（开发相关知识）
Servlet Tomcat JSP

传统XML配置SSM/SSH

SpringBoot

SpringCloud （了解即可）

# 反射
反射调用方法

反射修改字段

反射修改final的问题

进阶：高版本绕过反射限制等（有黑名单限制如何绕过）

# ASM/Javassist
(推荐用到再学，主要是安全开发需要学)

字节码是什么

如何用asm修改字节码

如何使用javassist生成字节码

# jndi攻击（重点）
8u191以上如何攻击

8u191以上如何打（反序列化/本地工厂）

如何审计这种漏洞

> [JNDI注入原理及利用考究](https://xz.aliyun.com/t/12277?time__1311=GqGxRDcD9D2iqGN4mxU2m7waPmThbD)
> 
> [JNDI注入分析](https://tttang.com/archive/1611/)
> 
> [素十八JNDI注入--Log4j2：里程碑式的顶级供应链漏洞](https://su18.org/tag/3WtBYGru6/)
# rmi攻击（重点）
rmi是什么

攻击Server端

攻击Register端

攻击Client端

攻击DGC
> [Java RMI 攻击由浅入深](https://su18.org/post/rmi-attack/)
> [Java安全学习——利用RMI进行攻击](https://goodapple.top/archives/520)

# java agent
启动前与运行中的Agent

Rasp的原理，简单实现

# JMX/JDWP
jmx/jdwp利用

# 反序列化基础（重点）
urldns/cc/cb/7u21/8u20 分析

尝试阅读并魔改ysoserial

JEP 290是什么

JEP 290鸡肋绕过

#fastjson反序列化（重点）
1.2.47以前的分析和绕过

1.2.47到1.2.68的分析和绕过

1.2.80的分析

利用方面（出网以及不出网）

# Weblogic
反序列化漏洞

二次反序列化

14882绕过

XML Decoder

IIOP/T3

文件上传

# Xstream/Jackson
他们历史上有很多Gadget

重点放在如何去找新的Gadget

# Hessian
dubbo历史上的一些洞

# SnakeYAML
SnakeYAML的利用（Jar）

SnakeYAML如何修复的

如何审计这种（SafeConstructor）

# Shiro （重点）
Shiro经典RCE

Shiro 721 Padding Oracke

如何检测（SimplePrincipalCollection）

如何自己写利用工具（加密）

如何通过Shiro注入内存马（内存马后文讲）

如何通过Shiro漏洞修改KEY

请求投过大限制的办法

对请求头长度严格限制情况下的绕过思路

存在Nginx反代和负载均衡下的问题解决

# Struts2
几十个漏洞

Spring（重点）
（Spring各种框架漏洞）

Spring RCE 分析

Spring EL相关漏洞 （Gateway Function Data）

SpringBoot Actuator 利用

Spring-Security相关的绕过

# Tomcat
Tomcat PUT rce

Tomcat CGI servlet rce

Tomcat session rce

Tomcat AJP rce

Tomcat 其他鸡肋洞

# 内存马原理（重点）
Servlet/Filter/Listener

Valve/WebSocket/Executor

Spring Controller/Interceptor

如何自己找内存马（核心context）

进阶内存马：Agent内存马，zhouyu内存马

内存马持久化

内存马反查杀（如何防止被检测到）

# 内存马查杀
c0ny1师傅的jsp查杀

核心：类名；存在文件

dump class查杀

sa-jdi dump agent

# log4j2
最初版RCE与RCE绕过姿势

2.15版本特殊绕过（特殊操作系统）

拒绝服务的原理

几种修复方案（以洞修洞）

java Agent修复

如何编写Burp插件来检测

#其他组件漏洞
Apache Solr

Apache Flink

Apache Spark

Apache Skywalking

# 进阶
tabby

codeql

自己分析字节码

自己写JVM


# 相关链接：
[Java Web安全](https://www.javasec.org/)

[java学习路线](https://www.viewofthai.link/2023/01/09/java-%E5%AE%89%E5%85%A8%E5%AD%A6%E4%B9%A0%E8%B7%AF%E7%BA%BF/)

[JAVA安全基础（一）--类加载器（ClassLoader）](https://xz.aliyun.com/t/9002?time__1311=n4%2BxnD0DuAitG%3DoqGNnmDUxYwKWqD5qP%2BKPQ34x)

[JAVA安全基础（二）-- 反射机制](https://xz.aliyun.com/t/9117?time__1311=n4%2BxnD0DuADtBrxBqooGkDRmxcnQ3kkHF4D)

[JAVA安全基础（三）-- java动态代理机制](https://xz.aliyun.com/t/9197?time__1311=n4%2BxnD0DuA0%3DiteGQ%3DDsA3EopG8iYkKDB7npoD)

[java靶场](https://github.com/j3ers3/Hello-Java-Sec)
[Hello Java Sec安全编码平台安装运行](https://cn-sec.com/archives/2313482.html)

[JAVA安全基础（四）-- RMI机制](https://xz.aliyun.com/t/9261?time__1311=n4%2BxnD0DuAG%3DQD5i%3DD%2FiW4BKGQkqYvXIjKqwKQx)

[java-代码审计学习篇](https://zone.huoxian.cn/d/736-java)

[网络安全零基础学习路线 ](https://www.processon.com/view/link/62b1b2267d9c08073c671315)
