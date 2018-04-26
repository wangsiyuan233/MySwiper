## 关闭浮层
### 任务一：关闭浮层

【平均用时 0.3 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%B8%80/%E5%85%B3%E9%97%AD%E6%B5%AE%E5%B1%82.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper//%E4%BB%BB%E5%8A%A1%E4%B8%80/%E5%85%B3%E9%97%AD%E6%B5%AE%E5%B1%82.html)

### 任务目的
1. 了解HTML的定义、概念、发展简史
2. 掌握常用HTML标签的含义、用法
3. 能够基于设计稿来合理规划HTML文档结构
4. 理解语义化，合理地使用HTML标签来构建页面

### 任务描述
- 本方案在点击时浮层弹出，同时开始监听 document 的点击事件。即在浮层出现的情况下才监听取消浮层事件，且事件只执行一次，执行之后就被回收，不会消耗太多内存。 

- setTimeout(function(){},0) 的作用是告诉JS引擎，完成当前的任务后立即开始执行function()。

-所以，在点击按钮之后，首先执行冒泡过程，冒泡完成之后，执行setTimeout的回调函数，添加document事件监听，此时添加的事件因为冒泡已经完成，不会在冒泡阶段被执行。

-重复开关按钮控制浮层。

### 任务注意事项

- 监听document事件只执行一次

