---
title: 函数声明和函数表达式的区别
categories:
  - 图解你不知道的JavaScript
tag:
  - 图解你不知道的JavaScript
---

## 1、形式上的区别

```js
// 函数声明
function mrfsm(greet) {
  return greet === 'hello Mr-fsm'
}
//函数表达式
var greet = function mrfsm(greet) {
  return greet === 'hello Mr-fsm'
}
```

## 2、在作用域上的区别

<img src="https://cdn.daddylab.com/Upload/image/20191023/1571793611435035.jpg" width="400" hegiht="250" align=center />

#### 函数声明在 JS 解析时进行函数提升，所以再同一个作用域，不管函数声明在哪里定义，该函数都可以进行调用，与此不同的是函数表达式的值是在 JS 运行时确定，并且在表达式赋值完成后，该函数才能调用。

## 总结

#### 函数声明是利用函数声明方法，其函数名就是申明中的函数名，声明具有函数提升效果

#### 函数表达式创建的函数是在运行时进行赋值，且要等到表达式赋值完成后才能调用

#### 两种的声明可能导致变量在不同作用域，从而引起不同效果，不注意的情况下，可能会引起意想不到的 bug

<!-- Link Gitalk 的支持文件  -->
<link rel="stylesheet" href="https://unpkg.com/gitalk/dist/gitalk.css">
<script src="https://unpkg.com/gitalk@latest/dist/gitalk.min.js"></script> 
<div id="gitalk-container"></div>     
<script type="text/javascript">
    var gitalk = new Gitalk({
		clientID: `cb37a23bb8fcfb7580af`,
		clientSecret: `54b05f873b4aa80c68edefb369951131abee5aea`,
		repo: `Mr-FSM.github.io`,
		owner: 'Mr-FSM',
		admin: ['Mr-FSM'],
		id: 'window.location.pathname'
    });
    gitalk.render('gitalk-container');
</script> 
<!-- Gitalk end -->
