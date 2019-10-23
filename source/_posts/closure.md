---
title: 一句话,一张图，轻松学闭包
categories:
  - 图解你不知道的JavaScript
tag:
  - 图解你不知道的JavaScript
---

### 一句话描述闭包

#### 用一个外层函数包裹全局变量,再用一个内层函数引用这个这个变量，然后外层函数返回内层函数，使得达到局部变量被重复使用的效果。

### 一张图解释闭包

<img src="https://cdn.daddylab.com/Upload/image/20191023/1571845435646870.jpg" width="400" hegiht="250" align=center />

<!-- Gitalk 评论 start  -->

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
