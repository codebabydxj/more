# webpack

> 模块化编程工具

## webpack和grunt、gulp有什么区别？

* Grunt和Gulp的工作方式是：在一个配置文件中，指明对某些文件进行类似编译，组合，压缩等任务的具体步骤，这个工具之后可以自动替你完成这些任务。

* Webpack的工作方式是：把你的项目当做一个整体，通过一个给定的主文件（如：index.js），Webpack将从这个文件开始找到你的项目的所有依赖文件，使用loaders处理它们，最后打包为一个浏览器可识别的JavaScript文件。

* 相对来说，webpack更方便更快捷，能打包更多文件。

### 安装

```
// 接管
npm init;
```

> 必须全局安装才能执行webpack命令，否则找不到

```
//全局安装
npm install -g webpack
//安装到你的项目目录
npm install --save-dev webpack
```

> 执行webpack命令

```
在接管文件夹下执行
webpack {entry file/入口文件} {destination for bundled file/存放bundle.js的地方}
```



