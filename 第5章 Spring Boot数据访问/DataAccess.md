# 第5章 Spring Boot 数据访问

Spring Boot 在数据访问方面，做了大量的封装、整合、集成工作。

在 Spring Boot 官方[start.spring.io](http://start.spring.io/) 中的 SQL 分类下有16个 starter，为开发人员提供了数据库访问方方面面的支持，极大的简化了开发配置工作。

![image-20191116220043447](images/image-20191116220043447.png)

从常见数据库的驱动依赖到 JDBC API（通过 jdbcTemplate）再到 MyBatis 持久 ORM 框架，都提供了完善的 starter 支持。还进一步提供了 Spring Data 项目在 SQL 方面的支持。

> Spring Data 的任务是为数据访问提供一个熟悉的、一致的、基于 Spring 的编程模型，同时仍然保留底层数据存储的特殊特性。
>
> 它使使用数据访问技术、关系数据库和非关系数据库、map-reduce 框架以及基于云的数据服务变得容易。这是一个伞形项目（umbrella project），包含许多特定于给定数据库的子项目。这些项目是通过与这些令人兴奋的技术背后的许多公司和开发人员合作开发的。

本章，我们会从最简单的 jdbcTemplate 开始介绍，然后介绍 MyBatis 集成及其分页插件。出于分享的目的，最后简要介绍了 MyBatis 加强框架（MyBatis-Plus），感兴趣的同学可以参照其官方文档进行系统性学习。

本章不介绍 Spring Data JPA 方面的内容，虽然其是一个非常强大的框架，提供了非常多的“基于约定”的数据库操作。但正是因为其封装“厚实”，不便于开发过程中对其进行细微调整，也不便于 DBA 对整个组织、整个项目的数据库架构设计进行规范化管理，所以我们在实际项目中使用得非常少。

当然，后续我们介绍 Spring Boot 对 NoSQL 方面的支持时，会使用 Spring Data Redis、Spring Data MongoDB 这些启动器的。
