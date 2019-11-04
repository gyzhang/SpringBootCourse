# 第4章 Spring Boot Web开发

Spring 框架提供了构建 Web 应用程序的全功能 MVC 模块。使用 Spring 可插入的 MVC 架构，可以选择是使用内置的 Spring Web 框架还是 Struts 这样的 Web 框架。通过策略接口，Spring 框架是高度可配置的，而且包含多种视图技术，例如 JavaServer Pages（JSP）技术、Velocity、Tiles、iText 和 POI。Spring MVC 框架并不知道使用的视图，所以不会强迫您只使用 JSP 技术。Spring MVC 分离了控制器、模型对象、分派器以及处理程序对象的角色，这种分离让它们更容易进行定制。

Spring 的 Web MVC 框架是围绕 `DispatcherServlet` 设计的，它把请求分派给处理程序，同时带有可配置的处理程序映射、视图解析、本地语言、主题解析以及上载文件支持。默认的处理程序是非常简单的 `Controller` 接口，只有一个方法 `ModelAndView handleRequest(request, response)`。Spring 提供了一个控制器层次结构，可以派生子类。如果应用程序需要处理用户输入表单，那么可以继承 `AbstractFormController`。如果需要把多页输入处理到一个表单，那么可以继承 `AbstractWizardFormController`。