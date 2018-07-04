Vue + Express 前后端脚手架
=========================================

在原版本基础之上，修改了webpack的相关配置文件。使得项目可以运行build命令，编译vue相关代码。
前端部分增加了vue全家桶（vue-router，vuex）
后端express部分增加有history模式，支持前端路由。需要传统后端路由方式的话，请注释掉`server/index.js`中`app.use(history())`
重新修改了文件夹结构

#### 1.10 版本
- 去掉了相关UI组件的配置，如果需要进行配置的话可以参考官方资料
  - [iView](https://www.iviewui.com/)
  - [element-UI](http://element-cn.eleme.io/#/zh-CN)
- 删除了不需要的package

fork源：[southerncross/vue-express-dev-boilerplate](https://github.com/southerncross/vue-express-dev-boilerplate)

## 关键词

- Vue (vue-router + vuex)
- Express
- Nodemon
- Webpack
- Npm


## 文件目录

```
.
├── LICENSE
├── README.md
├── nodemon.json
├── package.json
├── src
│   ├── client
│   │   ├── App.vue
│   │   ├── components
│   │   │   └── Hello.vue
│   │   │── static
│   │   │── router
│   │   │── store
│   │   │── views
│   │   └── index.js
│   └── server
│       ├── index.js
│       ├── config
│       ├── dao
│       ├── model
│       ├── router
│       ├── public
│       │   └── favicon.ico
│       └── views
│             └── index.html
├── build
│   ├── build.js
│   ├── clicheck-version.js
│   ├── dev-client.js
│   ├── utils.js
│   ├── vue-loader.conf.js
│   ├── webpack.base.conf.js
│   ├── webpack.dev.conf.js
│   └── webpack.prod.conf.js
├── config
     ├── dev.env.js
     ├── index.js
     └── prod.env.js
```

## 用法

1. 安装依赖包

   `npm install`

2. 运行开发环境

   `npm run dev 或者 npm start` 

3. build前端代码

    `npm run build`
    
    生成后的代码会在根目录的dist目录下。
    此时可专门写一个生产环境启动express的脚本。

## 参考资料

Some ideas are stolen from them, really appreciated.

- [Eslint guide](http://eslint.org/docs/user-guide/getting-started)
- [Express generator](http://expressjs.com/en/starter/generator.html)
- [Vue template](https://github.com/vuejs-templates/webpack)
- [Nodemon doc](https://github.com/remy/nodemon#nodemon)
- [Babel register](http://www.ruanyifeng.com/blog/2016/01/babel.html)
- [webpack-dev-middleware-boilerplate](https://github.com/madole/webpack-dev-middleware-boilerplate/tree/master/src)
- [how-can-i-use-webpack-with-express](http://stackoverflow.com/questions/31102035/how-can-i-use-webpack-with-express)
- [The-ultimate-webpack-setup](http://www.christianalfoni.com/articles/2015_04_19_The-ultimate-webpack-setup)
