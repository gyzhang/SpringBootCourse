



node-v12.15.0-x64.msi

https://gitee.com/sendya/ant-design-pro-vue/

https://pro.loacg.com/



yarn-1.22.0.msi

https://classic.yarnpkg.com/en/docs/install#windows-stable

https://classic.yarnpkg.com/latest.msi



安装完 yarn 后，使用国内淘宝镜像库，加快速度。

```
yarn config set registry https://registry.npm.taobao.org
```

创建前端脚手架项目

```powershell
git clone --depth=1 https://github.com/sendya/ant-design-pro-vue.git ant-pro-vue
```

```bash
├── public
│   └── logo.png             # LOGO
|   └── index.html           # Vue 入口模板
├── src
│   ├── api                  # Api ajax 等
│   ├── assets               # 本地静态资源
│   ├── config               # 项目基础配置，包含路由，全局设置
│   ├── components           # 业务通用组件
│   ├── core                 # 项目引导, 全局配置初始化，依赖包引入等
│   ├── router               # Vue-Router
│   ├── store                # Vuex
│   ├── utils                # 工具库
│   ├── locales              # 国际化资源
│   ├── views                # 业务页面入口和常用模板
│   ├── App.vue              # Vue 模板入口
│   └── main.js              # Vue 入口 JS
│   └── permission.js        # 路由守卫(路由权限控制)
├── tests                    # 测试工具
├── README.md
└── package.json
```



```powershell
cd .\ant-pro-vue\
yarn install
yarn run serve
```



![image-20200211125504119](images/image-20200211125504119.png)



[http://localhost:8000/](http://localhost:8000/)

![image-20200211125716324](images/image-20200211125716324.png)

用户名 admin 密码 ant.design 登录系统，主页工作台效果如下：

![image-20200211131809485](images/image-20200211131809485.png)