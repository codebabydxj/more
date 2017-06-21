### 回调函数

```
function async1(){
  //do sth...
}
function async2(){
  //do sth...
  async1();
}
async2();
```

> 只适合少量代码的时候，嵌套过多大大降低可读性。



