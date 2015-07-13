# 前端面试题总结

包括笔者本人遇到过的、网上见到过的以及自己想出来的各类前端相关的面试题。

部分参考文献如下：
- [Front-end Job Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions)
- [百度 FEX 团队面试题](https://github.com/fex-team/interview-questions)
- [阿里航旅事业部前端开发校招（电面）面试题](https://github.com/jayli/jayli.github.com/issues/19)
- [That JS Dude](http://thatjsdude.com/interview/index.html)

## 题目列表

- HTML
    + DOCTYPE 声明的取值与区别
    + 常见的 meta 标签有哪些？移动端呢？
    + 关于 HTML 语义化知道哪些？
    + 是否有关注 HTML 标准的演进？比较关注哪些方面？能否举一些例子？
- CSS
    + 盒模型、IE 6/7 与现代浏览器的区别、如何兼容
    + BFC/IFC/Flexbox 的概念
    + containing block 和 stacking context 的概念和计算
    + position 和 display 的取值和各自的意思和用法
    + 如何清除浮动？为什么要清除浮动？
    + 不同浏览器上的默认样式，如何处理？（normalize/sanitize）
    + 选择器
        * specificity
        * 伪类和伪元素的区分
        * 选择器性能（浏览器如何进行匹配）
        * CSS3 和 CSS4 选择器知道哪些
    + CSS 优化
        * 网络加载方面有哪些手段
        * 渲染性能的方面呢
    + 用过哪些 CSS 方面的工具
    + 随便谈谈 CSS 工程化
- JavaScript & DOM
    + 有哪些基本类型
    + 区分不同类型的方法有哪些，各有什么问题
    + 闭包的概念 & 用途
    + `apply` 和 `call` 的用途和区别
    + 原型继承的概念， `prototype` 和 `__proto__` 的区别
    + 是否碰到过内存泄露？能否说一下引起内存泄露的常见原因（网上大部分文章都是跟 IE 相关的，其实没什么必要了解，闭包方面有必要知道）？有什么工具可以调试？
    + JavaScript 模块化
        * 常见规范
        * 工具
        * 实现原理
    + DOM 的事件机制
        * 冒泡与捕获的概念，如何阻止冒泡
        * Delegation
        * 鼠标点击 a 标签其中会有多少个时间产生
        * 如何区分 dbclick 和 click
    + ajax 请求中 readyState 有哪些状态（这个问题我感觉太不常考了……但既然见到过那就收录进来了）
    + ajax 跨域
        * 怎样算是跨域？
        * 跨域的方法有哪些？实现原理是什么？兼容性如何？各自有什么缺点？
        * JSONP 如果页面编码和被请求的资源编码不一致如何处理
    + 服务器端消息推送有哪些方法？实现原理？兼容性？缺点？
    + jQuery.ready() 实际上是 DOM 中的什么事件？
    + JavaScript 设计模式知道哪些？Proxy 模式怎么用？
    + ES6 是否有了解
- 前端性能优化
    + 雅虎 24 条，说出越多越好
    + 是否听说过 BigPipe（这个我自己加的，没见人问过）
- 页面性能分析
    + 页面性能一般可以有哪些指标
    + 页面性能记录和分析有哪些方法？除了常见的那些方法之外在现代浏览器里还有其他什么新手段吗？
    + 用过什么性能分析的工具
- 前端安全
    + XSS 的概念、知道哪些解决办法（常规的就行，不必太深入）
    + CSRF 攻击的概念、防御手段
- 后端
    + 讲讲 session 的实现原理
    + 讲讲 RESTful
- NodeJS
    + callback hell 以及目前的解决方案
- 网络
    + TCP 三次握手
        * 具体过程
        * 为什么要这么设计
    + 说一下网络五层模型（HTTP协议从应用层到底层都基于哪些协议），HTTP 协议头字段说上来几个，缓存字段是怎么定义的，http和https的区别，在具体使用的时候有什么不一样。是否尽可能详细的掌握HTTP协议
    + HTTP 状态码
        * 1、2、3、4、5 开头分别表示什么
        * 301 和 302 的区别、为什么要区分
    + cookies 是干嘛的，服务器和浏览器之间的 cookies 是怎么传的，httponly 的 cookies 和可读写的 cookie 有什么区别，有无长度限制，cookies 被禁用后可以考虑用什么替代
- 其他
    + 会不会用 ps 扣图，png、jpg、gif 这些图片格式解释一下，分别什么时候用。是否了解webp
    + 是否了解开源的工具 bower、npm、yeoman、grunt、gulp，有无用过，有无写过，一个 npm 的包里的 package.json 具备的必要的字段都有哪些（名称、版本号，依赖）
- 手写代码
    + walkTheDOM 函数，从 `<body>` 标签起，遍历所有节点并打印标签名
    + 实现一个简单的 pub-sub 库
    + 实现 `_.flatten()`
    + object deep clone
    + isPrime
    + quicksort
    + mergesort
    + binary search
    + throttle & debounce
    + 实现 `Object.create()`（不用完全遵循标准，实现蝴蝶书上的版本就够了）
    + Function.prototype.bind
    + 实现一个圣杯布局
    + carousel 组件
    + 自动补全组件
    + overlay 组件
    + popup 组件
- 算法题
    + topK
    + 翻转单链表
    + 反转二叉树
    + 单向列表判断是否有环
    + [LeetCode](https://leetcode.com/)
    + [careercup](http://www.careercup.com/)
    + [结构之法 算法之道](http://blog.csdn.net/v_JULY_v)
