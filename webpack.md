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

### 执行webpack

#### 1. 命令行执行

```
// 局部
.\node_modules\.bin\webpack app/index.js dist/bundle.js
// 全局
webpack app/index.js dist/bundle.js
// webpack命令 入口 出口
```

#### 2. 配置文件执行

根目录下创建webpack.config.js文件，规范代码如下：

```
var path = require('path');

module.exports = {
  // 入口
  entry: './app/index.js',
  // 出口
  output: {
    filename: 'bundle.js',
    path: path.resolve(__dirname, 'dist')
  }
};
```

通过命令行执行此文件即可。

```
webpack --config webpack.config.js
```

#### 3. 设置快捷方式

在package.json文件的scripts中加入快捷方式：

```
"build": "webpack"
```

执行如下命令即可。

```
npm build
```



