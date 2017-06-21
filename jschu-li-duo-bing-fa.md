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

### ajax改为同步

```
$.ajax({
  url:"/jquery/test1.txt",
  async:false
});
```

### 回调计数

```
var cnt = 0;
function async1(){
  //do sth...
  callback();
}
function async2(){
  //do sth...
  callback();
}
function callback(){
  cnt++;
  if(2==cnt) console.log('都已执行完毕');
```



