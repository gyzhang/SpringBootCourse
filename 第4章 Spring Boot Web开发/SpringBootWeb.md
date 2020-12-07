# 第4章 Spring Boot Web 开发

Spring Boot 针对 Web 应用开发，从开发、测试和部署都做了全面地支持，堪称完美。

`spring-boot-starter-web` 是 Spring Boot 对 Web 开发提供支持的起步依赖，主要包括开发 RESTful 服务的支持、参数校验、使用 Tomcat/Jetty/Undertow 作为内嵌 web 容器等功能。

通常情况下，我们会通过 Spring Boot 使用 Spring MVC 模块来支持 web 开发。

> 当前，使用 Spring MVC 最简单直接，也是最广泛的方式就是使用 Spring Boot 的起步依赖。

在众多的 Web MVC 框架中，Spring MVC 是独树一帜的：方便、高效、够用、和 Spring 原生集成。所以在和前辈 Struts、官方 Java Serve Faces 的竞争中脱颖而出，几乎成了当前 Java EE 应用中事实上的 MVC 标准。

本章，我们会先介绍 Spring MVC 的特点，结合 Spring Boot 如何方便地开发 RESTful 风格的应用。

然后介绍 Spring 推荐的、替代 JSP 的模板引擎 Thymeleaf（虽然并不好用），并做简单整合示例。

> Thymeleaf 在做 Web 页面引擎方面实际上也不咋样，还有一个不错的引擎 pebbletemplates，可以尝试。

最后介绍传统 Servlet、Listener、Filter 和 JSP 技术如何在 Spring Boot 中使用，以便兼容以前的遗留应用。

> 为什么还要介绍传统的 Servlet 技术？
> 因为在重要的生产系统中，祖传代码还是蛮多的。
