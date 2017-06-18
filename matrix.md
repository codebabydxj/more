# matrix

> 矩阵算法

```
[a,c,e]   [x]
[b,d,f] * [y] 
[0,0,1]   [1]
```

### 偏移（translate）

* ax+cy+1e=x轴的偏移量
* bx+dy+1f=y轴的偏移量

> eg:x偏移30px,y偏移50px

```
// 1*0+0*0+30*1=x
// 0*0+1*0+50*1=y
transform:matrix(1,0,0,1,30,50)
```



