# 微信小程序之flex布局

## 一、 小程序代码编写规范

代码编写的规范每个公司都不太一样，但是每个公司都有一套自己的代码约束规范，但是有以下几点需要大家注意：

- 定义的规范不能引起代码的错误
- 遵循大的规范

## 二、 什么是布局？

![image-20191125190850391](/Users/yangling/Library/Application Support/typora-user-images/image-20191125190850391.png)

## 三、 block，inline与inline-block

![image-20191125191614137](/Users/yangling/Library/Application Support/typora-user-images/image-20191125191614137.png)

![image-20191125191417524](/Users/yangling/Library/Application Support/typora-user-images/image-20191125191417524.png)

## 四、 flex容器将消除item的块状特性

水平排列：

```
display:flex;
```



## 五、 flex-direction的应用

水平排列：

```
flex-direction:row;
```

垂直排列：

```
flex-direction:column;
```



## 六、 reverse倒序排布

色块水平方向颠倒：

```
flex-direction：row-reverse;
```

色块垂直方向颠倒：

```
flex-direction：column-reverse；
```



## 七、 reverse倒叙排序

问题： view的高度是自适应

解决方案： 给view设置高度

## 八、 justify-content属性解析(一)

对齐方向：

- 逆向排序，向上对齐

- ```
  justify-content: flex-end;
  ```

- 逆向排序，向下对齐

- ```
  justify-content: flex-start;
  ```

- 正向排序，向上对齐

- ```
  justify-content: flex-start;
  ```

- 正向排序，向下对齐

  ```
  justify-content： flex-end;
  ```

水平方向和上面同理



## 九、 justify-content属性解析(二)

- 水平居中对齐

  ```
  justify-content:center;
  ```

- 两端对齐(平均分布)

- ```
  justify-content:space-brtween;
  ```

- 等距分布

  ```
  justify-content:space-around;
  ```

  

## 十、 主轴与交叉轴

- 设置元素垂直排列，并垂直居中，且水平居中

- ```
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  ```

  一旦确定主轴和交叉轴，那么justify-content设置的就是主轴，align-items设置的就是交叉轴

## 十一、 base1line与stretch

## 十二、 flex-wrap与消除间距