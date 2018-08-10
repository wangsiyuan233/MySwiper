# 轮播合集总结

## 关闭浮层
### 任务一：关闭浮层

【平均用时 0.3 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%B8%80/%E5%85%B3%E9%97%AD%E6%B5%AE%E5%B1%82.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper//%E4%BB%BB%E5%8A%A1%E4%B8%80/%E5%85%B3%E9%97%AD%E6%B5%AE%E5%B1%82.html)

### 任务目的
1. 了解冒泡过程
2. 简单运用JQ
3. 了解setTimeout
4. 绑定document

### 任务描述
- 本方案在点击时浮层弹出，同时开始监听 document 的点击事件。即在浮层出现的情况下才监听取消浮层事件，且事件只执行一次，执行之后就被回收，不会消耗太多内存。 

- setTimeout(function(){},0) 的作用是告诉JS引擎，完成当前的任务后立即开始执行function()。

- 所以，在点击按钮之后，首先执行冒泡过程，冒泡完成之后，执行setTimeout的回调函数，添加document事件监听，此时添加的事件因为冒泡已经完成，不会在冒泡阶段被执行。

- 重复开关按钮控制浮层。

### 任务注意事项

- 监听document事件只执行一次

- 伪元素不属于文档，所以js无法操作它

	伪元素属于主元素的一部分，因此点击伪元素触发的是主元素的click事件

	原文说块级元素才能有:before, :after，其实是不妥的，大部分行级元素也可以设置伪元素，但是像img可替换元素，因为其外观和尺寸有外部资源决定，那么如果外部资源正确加载，就会替换掉其内部内容，这时伪元素也会被替换掉，但是当外部资源加载失败时，设置的伪元素是可以起作用的。


### 任务二：普通轮播

**▲普通轮播1**

【平均用时 0.2 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%BA%8C%EF%BC%9A%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD/%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD1.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper/%E4%BB%BB%E5%8A%A1%E4%BA%8C%EF%BC%9A%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD/%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD1.html)

### 任务目的
Jquery绑定click事件

### 任务描述
完成最简单的手动切换图片


**▲普通轮播2**

【平均用时 0.3 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%BA%8C%EF%BC%9A%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD/%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD2.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper/%E4%BB%BB%E5%8A%A1%E4%BA%8C%EF%BC%9A%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD/%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD2.html)

### 任务目的
自动轮播+button也随着切换在变红

### 任务描述 
简单的意识流写法，没有函数的封装


**▲普通轮播3**

【平均用时 0.4 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%BA%8C%EF%BC%9A%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD/%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD3.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper/%E4%BB%BB%E5%8A%A1%E4%BA%8C%EF%BC%9A%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD/%E6%99%AE%E9%80%9A%E8%BD%AE%E6%92%AD3.html)

### 任务目的
自动轮播+button也随着切换在变红

### 任务描述 
将重复的代码封装到不同的函数当中，函数中调用函数。

## 无缝轮播
### 任务三：无缝轮播

**▲无缝轮播1**

【平均用时 0.2 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%B8%89%EF%BC%9A%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD/%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD1.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper/%E4%BB%BB%E5%8A%A1%E4%B8%89%EF%BC%9A%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD/%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD1.html)

### 任务目的
Jquery实现无缝轮播

### 任务描述
- 确定图片数量


**▲无缝轮播2**

【平均用时 0.3 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%B8%89%EF%BC%9A%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD/%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD2.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper/%E4%BB%BB%E5%8A%A1%E4%B8%89%EF%BC%9A%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD/%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD2.html)

### 任务目的
Jquery实现无缝轮播

### 任务描述 
- 确定图片数量



**▲无缝轮播3**

【平均用时 0.4 天】
[【我的代码】](https://github.com/wangsiyuan233/MySwiper/blob/master/%E4%BB%BB%E5%8A%A1%E4%B8%89%EF%BC%9A%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD/%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD3.html)
[【效果预览】](http://wangsiyuan233.cn/MySwiper/%E4%BB%BB%E5%8A%A1%E4%B8%89%EF%BC%9A%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD/%E6%97%A0%E7%BC%9D%E8%BD%AE%E6%92%AD3.html)

### 任务目的
Jquery实现无缝轮播

### 任务描述 
- 确定图片数量
- offset函数