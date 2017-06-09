## AMD&CMD

> 模块化开发和编程

#### AMD——requery.js

> 依赖前置，提前执行，2.0之后可以依赖就近

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



