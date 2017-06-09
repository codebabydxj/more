## AMD&CMD

> 模块化编程的方法

#### AMD

> 依赖前置，提前执行，2.0之后可以依赖就近

##### require.js

```
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


