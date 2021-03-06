# matrix

> 矩阵算法

```
[a,c,e]   [x]
[b,d,f] * [y] 
[0,0,1]   [1]
```

### 偏移（translate）

> 只需要关注最后两个参数

* ax+cy+1e=x轴的偏移量
* bx+dy+1f=y轴的偏移量

> eg:x偏移30px,y偏移50px

```
// 1*x+0*y+30*1=x
// 0*x+1*y+50*1=y
transform:matrix(1,0,0,1,30,50)
```

> 为什么a和d是1呢？
>
> 是为了控制缩放的两个值，如果成为0，将无法显示

### 缩放（scale）

> 只需要关注a和d两个参数，同偏移公式一样
>
> eg:x放大3倍，y放大2倍

```
transform:matrix(3,0,0,2,0,0);
```

### 旋转（rotate）

> 使用到三角函数

* x\*cos\(\)-y\*sin\(\)
* x\*sin\(\)+y\*cos\(\)

```
cosVal = Math.cos(this.value * Math.PI / 180);
sinVal = Math.sin(this.value * Math.PI / 180);
matrix(cosθ,sinθ,-sinθ,cosθ,0,0);
```

> eg:旋转30度

```
transform:matrix(0.866025,0.500000,-0.500000,0.866025,0,0);
```

### 倾斜（skew）

> 使用tan\(\)，同旋转原理一样

```
tanValY = Math.tan(eleRangeY.value * Math.PI / 180);
tanValX = Math.tan(eleRangeX.value * Math.PI / 180);
matrix(1,tan(θy),tan(θx),1,0,0);
```

> eg:倾斜30度

```
transform:matrix(1,0.000000,0.839100,1,0,0);
```



