## AMD&CMD

> 模块化开发和编程

#### AMD——require.js

> 依赖前置，提前执行，2.0之后可以依赖就近

```
// html引入
<script data-main="index.js" src="require.js" async="async" defer></script>
// js中使用
define(["a","b"],function(a,b){//函数体})
```

#### CMD

> 依赖就近，延迟执行

##### sea.js

```
define(function(require,exports,module){
    var a=require("./a");
    //函数体
})
```



