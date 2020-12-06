# Spring Boot 培训教程

这是一套 Spring Boot 的快速入门培训教程，面向的学员是有一定的 Java 基础，会一些 Spring 传统开发技能（SSM）的初中级 Java 开发工程师。

其目的是通过2-3个月的时间，每周完成1章节的教程学习（可能需要在一个学习小组内，通过辅导教员引导），达到能够应用 Spring Boot 进行开发的程度，向中级开发工程师进阶，进而打好后续学习 Spring Cloud 的基础。

虽然本教程提供了一个极简的 vue 入门学习章节，其目的只是用来演示如何开发“前后端分离”的应用，但是本教程并不会将前端开发作为重点。相反，在这里，我们只关心应用后端如何使用 Spring Boot 进行开发。

本教程规划于2019年春，动笔于2019年10月30日，希望完结于2019年12月31日，实际完结于2020年2月7日，历时101天，我也坚持连续写作101天。

>任何时候出发，都不晚，相信我，风景总是在路上。
>
>--Kevin Zhang

- 本教程使用的 Spring Boot 版本为[2.2.1-2.2.4](https://github.com/spring-projects/spring-boot/tree/v2.2.4.RELEASE)；

> 写作过程中，Spring Boot 从2.2.1持续升级到了2.2.4，可见 Spring  Boot 社区的活跃。

- 本教程的每一章节，尽量聚焦在当前讨论的知识点范围内，示例也设计为最简；

- 本教程不涉及 Spring Boot 的深层次实现机制和如何扩展 Spring Boot 框架；

- 已经能够熟练使用 Spring Boot 进行开发的同学，请绕道，这份教程不适用于你。

如何将本书编译成 pdf、epub 等电子书格式？

1. 先到 [https://nodejs.org/en/](https://nodejs.org/en/) 下载 node.js LTS（[node-v12.16.0-x64.msi](https://nodejs.org/dist/v12.16.0/node-v12.16.0-x64.msi)） 版，安装；
2. 打开命令行窗口输入命令 `npm i -g gitbook-cli` 安装 gitbook 环境；
3. 然后到 [https://calibre-ebook.com/](https://calibre-ebook.com/) 下载 [calibre 3.40.1](https://download.calibre-ebook.com/3.40.1/calibre-64bit-3.40.1.msi) 并安装。需要注意的是最新版本和 gitbook 不兼容；
4. 将本教程的版本库下载或克隆到本地；
5. 打开命令行窗口，进入 SpringBootCourse 版本库目录；
6. 执行 `gitbook install` 安装 gitbook 插件；
7. 执行 `gitbook pdf` 生成本书的 pdf 版本；
8. 执行 `gitbook epub` 生成本书的 epub 电子书。
