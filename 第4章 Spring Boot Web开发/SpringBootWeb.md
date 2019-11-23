# 第4章 Spring Boot Web开发

Spring Boot针对Web应用开发，从开发、测试和部署都做了全面地支持，堪称完美。

`spring-boot-starter-web`是Spring Boot对Web开发提供支持的启动器，主要包括开发RESTful服务的支持、参数校验、使用 Tomcat/Jetty/Undertow作为内嵌容器器等功能。

通常情况下，我们会通过Spring Boot使用Spring MVC模块来支持web开发。

在众多的web MVC框架中，Spring MVC是独树一帜的：方便、高效、够用、和Spring原生集成。所以在和前辈Struts、官方Java Serve Faces的竞争中脱颖而出，几乎成了当前Java EE应用中事实上的MVC标准。

本章，我们会先介绍Spring MVC的特点，结合Spring Boot如何方便地开发RESTful风格地应用。

然后介绍Spring推荐地、替代JSP的模板引擎Thymeleaf，并做简单整合示例。

最后介绍传统Servlet、Listener、Filter和JSP技术如何在Spring Boot中使用，以便兼容以前的遗留应用。

