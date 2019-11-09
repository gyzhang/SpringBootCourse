# Spring Boot 培训教程

这是一套Spring Boot的快速入门培训教程，面向的学员是有一定的Java基础，会一些Spring传统开发的初级Java开发工程师。

其目的是通过2-3个月的时间，每周完成1章节的教程学习（可能在一个学习小组内需要辅导教员引导），达到能够应用Spring Boot进行开发的程度，向中级开发工程师进阶。

虽然本教程提供了一个极简的vue入门学习章节，其目的是用来演示如何开发“前后端分离”的应用。本教程并不会将前端开发作为重点。相反，在这里，我们只关心后端如何使用Spring Boot进行开发。

本课程规划于2019年春，动笔于2019年10月30日，希望完结于2019年12月31日。

>任何时候出发，都不晚，相信我，风景总是在路上。
>
>--Kevin Zhang

- 本教程使用的Spring Boot版本为[2.2.1](https://github.com/spring-projects/spring-boot/tree/v2.2.1.RELEASE)；
- 本教程的每一章节尽量聚焦在当前讨论的知识点范围内，示例也设计为最简；
- 本教程不涉及Spring Boot的深层次实现机制和如何扩展Spring Boot框架；
- 已经能够熟练使用Spring Boot进行开发的同学，请绕道，这份教程不适用于你。

本教程使用GitBook开发，其**book.json**配置信息如下：

```json
{
    "title": "SpringBoot入门教程",
    "description": "针对初级程序员的Spring Boot入门教程，使用版本2.2.1",
    "author": "Kevin Zhang",
	"language": "zh-hans",
	
	"plugins": [ 
		"-search",
		"search-pro",
		"code",
		"splitter",
		"expandable-chapters",
		"page-toc-button",
		"back-to-top-button"
	],
	
	"pluginsConfig": {
		"search-pro": {
			"cutWordLib": "nodejieba",
			"defineWord": ["Spring Boot"],
			"expandable-chapters":{}
		}
	},
	
	"pdf": {
		"paperSize": "a4",
		"fontSize": 30		
	}
}
```

