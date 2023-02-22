#### CSS盒子模型：

盒子组成部分：content，padding，border，margin

模式：

- 标准盒子模型content-box

- ie盒子模型border-box

默认为content-box

###### 控制：

box-sizing

###### 区别：

- content-box：padding和border不被包含在定义的width和height之内
-  border-box：padding和border包含在定义的width和height之内



###### tip：

设置width和height为0px，利用盒模型中的border来实现三角形。

```
div{
	width: 0px;
	height: 0px;
	border: 100px solid;
	border-color: transparent transparent transparent red;
}
```

