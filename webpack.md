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

> 必须全局安装才能执行webpack，否则找不到指定的命令。

```
//全局安装
npm install -g webpack
//安装到你的项目目录
npm install --save-dev webpack
```

> 执行webpack命令，后两个参数第一个是要处理的文件，第二个是处理之后的文件。

```
在接管文件夹下执行
webpack {entry file/入口文件} {destination for bundled file/存放bundle.js的地方}
```

> > 另外

在package.json中写入：

```
"scripts": {
    "start": "webpack app/main.js public/bundle.js" //配置的地方就是这里啦，相当于把npm的start命令指向webpack命令
  },
```

相当于把这一行命令托付给start，只需要执行

```
npm start
```

就可以执行这一串代码。

### 创建本地服务器，自动化构建



