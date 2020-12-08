# 第16章 Spring Boot 综合示例

经过前面 15 章的学习，我们已经了解了 Spring Boot 的部分生态技术栈。

在本章，我们将通过 github 上开源的“[微人事](https://github.com/lenve/vhr)”项目来串接在本教程种学习到的各个知识点。

> 该项目的作者是**王松**，微信公众号**江南一点雨**，感谢作者开源的这个示例项目。

项目是一个常见的企业人事管理系统，功能包括机构、员工资料管理，人事管理，工资管理，沟通聊天室等。我们不去探讨如何实现业务功能，重点回顾如何集成我们需要的技术。

**项目后端技术栈：**Spring Boot、Spring Security、MyBatis、MySQL、Redis、RabbitMQ、Spring Cache、WebSocket...

**项目前端技术栈：**Vue、ElementUI、axios、vue-router、Vuex、WebSocket、vue-cli4...

在这一章中，我们会对项目的设计、关键配置、代码进行解读。为了更好地衔接后续 “Spring Cloud 培训教程” ，我们会使用 docker 容器来提供数据库、缓存和消息等服务。
