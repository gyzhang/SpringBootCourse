# 第12章 Spring Boot 安全控制

安全控制是企业应用中不可或缺的基础要求，也是隔离于具体业务需求之外而存在的一个基础技术服务。

[Spring Security](https://spring.io/projects/spring-security) 是  Spring 家族中的一个安全管理框架。实际上，在 Spring Boot 出现之前，Spring Security 就已经发展了很多年了，但是使用的并不多。在很长一段时间内，安全管理这个领域，一直是 Apache Shiro 的天下。

相对于 Shiro，在 SSM/SSH 中整合 Spring Security 是比较麻烦的操作。所以，Spring Security 虽然功能比 Shiro 强大，但是使用反而没有 Shiro 多（Shiro 虽然功能没有 Spring Security 多，但是对于大部分项目而言，Shiro 也够用了）。

自从有了 Spring Boot 之后，Spring Boot 对于 Spring Security 提供了 自动化配置方案，可以零配置使用 Spring Security，所以 Spring Security 才焕发了新的生机，再次流行起来。

在我们的日常工作，最常见的安全管理技术栈的组合是这样的：

- SSM + Shiro；
- Spring Boot/Spring Cloud + Spring Security；

本章围绕 Spring Security 展开介绍 Spring Boot 中的安全控制。我们首先介绍 Spring Security 的基本概念及其原理，然后介绍 Open Web 环境下的安全管控机制 OAuth 2，最后结合 CAS 介绍如何实现单点登录功能。

> 我在上一版的开发平台（JEP 5）中对安全控制框架做技术选型时，最主要的考量就是”够用，易用，大家都在用“，所以选了 Shiro。但是在最新的一版开发平台（iJEP 6）中安全控制框架选择了 Spring Security，而选型原则并没有改变，还是”够用，易用，大家都在用“。
>
> 那是因为托了 Spring Boot 的福：大大降低了 Spring Security 的使用门槛。

更多关于Spring Security 的学习材料，请参考这里：[https://www.baeldung.com/security-spring](https://www.baeldung.com/security-spring)
