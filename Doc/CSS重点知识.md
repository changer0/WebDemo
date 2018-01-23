# css重点知识

## 浮动
1. 浮动的元素会脱标
2. 目的：让多个块级元素浮动在同一行；
3. 取值：left；right；none；

### 清除浮动
1. 根据情况需要来清除浮动
2. 目的：为了解决父盒子高度为0的问题

#### 清除浮动的方式
1. 额外标签法
2. overflow：hidden；
3. 伪元素清除法(最常用)

```
    .clearfix:after{
        content:"";
        visibility:hidden;
        display:block;
        height:0;
        clear:both;
    }
```
4. 双伪元素

```
.clearfix:before, .clearfix:after{
    display: table;
    content:"";
}
.clearfix:after{
    clear: both;
}
```
## 鼠标样式
1. cursor:pointer; 鼠标变成小手的形状
2. cursor:default; 默认形状小箭头
3. cursor:move; 移动时显示的样式
4. cursor:text; 输入时显示光标的形状
