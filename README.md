# 前端面试题总结

包括笔者本人遇到过的、网上见到过的以及自己想出来的各类前端相关的面试题。

部分参考文章如下：

- [Front-end Job Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions)
- [百度 FEX 团队面试题](https://github.com/fex-team/interview-questions)
- [阿里航旅事业部前端开发校招（电面）面试题](https://github.com/jayli/jayli.github.com/issues/19)
- [That JS Dude](http://thatjsdude.com/interview/index.html)
- [前端开发面试题](https://github.com/markyun/My-blog/tree/master/Front-end-Developer-Questions/Questions-and-Answers)
- [FE-Interview](https://github.com/qiu-deqing/FE-interview)
- [如何面试 JS 开发工程师](http://www.zhihu.com/question/37441607)


## 题目列表

- HTML
    + [DOCTYPE 声明的作用、取值与区别](#html-doctype-声明)
    + [常见的 meta 标签有哪些？移动端呢？](#常见的-meta-标签)
    + [关于 HTML 语义化知道哪些？](#html-语义化)
    + [是否有关注 HTML 标准的演进？比较关注哪些方面？能否举一些例子？](#html-标准)
- CSS
    + CSS 有几种引入方式？各自的优缺点？
    + [盒模型、IE 6/7 与现代浏览器的区别、如何兼容](#css-盒模型)
    + BFC 的概念
    + containing block 和 stacking context 的概念和计算
    + [`position: absolute` 和 `float` 有什么区别](#absolute-和-float-的区别)
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
    + [JavaScript 有哪些基本类型](#javascript-基本类型)
    + 区分不同类型的方法有哪些，各有什么问题
    + 闭包的概念 & 用途
    + `apply` 和 `call` 的用途和区别
    + 原型继承的概念， `prototype` 和 `__proto__` 的区别
    + 是否碰到过内存泄露？能否说一下引起内存泄露的常见原因（网上大部分文章都是跟 IE 相关的，其实没什么必要了解，闭包方面有必要知道）？有什么工具可以调试？
    + JavaScript 设计模式知道哪些？Proxy 模式怎么用？
    + ES6 是否有了解
    + JavaScript 模块化
        * 常见规范
        * 工具
        * 实现原理
 - DOM
    + DOM 的事件机制
        * 冒泡与捕获的概念，如何阻止冒泡
        * Delegation
        * 鼠标点击 a 标签其中会有多少个时间产生
        * 如何区分 dbclick 和 click
    + ajax 请求中 readyState 有哪些状态（这个问题我感觉太不常考了……但既然见到过那就收录进来了）
    + ajax 跨域
        * 怎样算是跨域？
        * [跨域的方法有哪些？实现原理是什么？兼容性如何？各自有什么缺点？](#ajax-跨域)
        * JSONP 如果页面编码和被请求的资源编码不一致如何处理
    + [服务器端消息推送有哪些方法？实现原理？兼容性？缺点？](#服务器端推送)
    + jQuery.ready() 实际上是 DOM 中的什么事件？
- 前端性能优化
    + 雅虎 24 条，说出越多越好
    + 是否听说过 BigPipe（这个我自己加的，没见人问过）
- 页面性能分析
    + 页面性能一般可以有哪些指标
    + 页面性能记录和分析有哪些方法？除了常见的那些方法之外在现代浏览器里还有其他什么新手段吗？
    + 用过什么性能分析的工具
- 前端安全
    + XSS 的概念、知道哪些解决办法（常规的就行，不必太深入）
    + `escape` / `encodeURI` / `encodeURIComponent` 的区别
    + CSRF 攻击的概念、防御手段
- 后端
    + 讲讲 session 的实现原理，cookies 和 session 的关系，以及可否不用 cookies 实现
    + 多台服务器之间该如何共享 session
    + 讲讲 RESTful
- NodeJS
    + callback hell 以及目前的解决方案
    + 用过 koa 吗？thunk 是什么？（等 koa 2 正式版出来以后这个可以不用问了）
    + 什么是事件循环？Node 中有哪些类型的函数/调用是异步的？哪些是同步的？
    + 写过单元测试吗？用过什么库？
    + 怎样绑定 Node 程序到 80 端口[#绑定-node-程序到-80-端口]？
    + 有哪些方法可以让 Node 程序遇到错误后自动重启
    + 如何实现一个 writable stream？
- TypeScript
    + 都说 TypeScript 的类型系统是 unsound 的，请问这个 unsound 是什么意思？具体表现在什么地方？
    + `interface` 和 `declare class` 都可以用来描述一个类，请问这两者的区别是什么？
- 网络
    + TCP 三次握手
        * 具体过程
        * 为什么要这么设计
    + 说一下网络五层模型（HTTP 协议从应用层到底层都基于哪些协议），HTTP 协议头字段说上来几个，缓存字段是怎么定义的，http 和 https 的区别，在具体使用的时候有什么不一样。是否尽可能详细的掌握 HTTP 协议
    + HTTP 状态码
        * 1、2、3、4、5 开头分别表示什么
        * 301 和 302 的区别、为什么要区分
    + cookies 是干嘛的，服务器和浏览器之间的 cookies 是怎么传的，httponly 的 cookies 和可读写的 cookie 有什么区别，有无长度限制，cookies 被禁用后可以考虑用什么替代
- 其他
    + 会不会用 ps 扣图，png、jpg、gif 这些图片格式解释一下，分别什么时候用。是否了解webp
    + 是否了解开源的工具 bower、npm、yeoman、grunt、gulp，有无用过，有无写过，一个 npm 的包里的 package.json 具备的必要的字段都有哪些（名称、版本号，依赖）
    + 如何判定访问者的身份是同一人？除了 cookies 还有什么替代品？
- 手写代码
    + walkTheDOM 函数，从 `<body>` 标签起，遍历所有节点并打印标签名
    + addClass
    + 实现一个简单的 pub-sub 库
    + 实现 `_.flatten()`
    + object deep clone
    + isPrime
    + quick sort
    + merge sort
    + binary search
    + throttle & debounce
    + 实现 `Object.create()`（不用完全遵循标准，实现蝴蝶书上的版本就够了）
    + `Function.prototype.bind`
    + CSS 实现元素的水平垂直居中
    + 实现一个圣杯布局
    + carousel 组件
    + 自动补全组件
    + overlay 组件
    + popup 组件
    + drag & drop 组件，分别用 jQuery、MVVM、React 和 RxJS 实现一遍
    + [一小时之内写一个扫雷游戏](#一小时之内写一个扫雷游戏)
- 代码实现思路
    + 如果要你实现一个 AMD 加载器，你将如何实现？讲一下思路和需要注意的点，最好有伪代码
    + Sizzles （jQuery 的选择器模块）的实现思路
- 算法题
    + topK
    + 翻转单链表
    + 反转二叉树
    + 单向列表判断是否有环
    + [LeetCode](#leetcode)
    + [careercup](http://www.careercup.com/)
    + [结构之法 算法之道](http://blog.csdn.net/v_JULY_v)


## 答案


### HTML DOCTYPE 声明

[HTML 4.01 和 XHTML 都基于 SMGL](http://www.w3.org/TR/REC-html40/intro/sgmltut.html)，所以需要在文档开头声明引用一个 DTD。

在 HTML 5 中，DOCTYPE 不区分大小写；不过对于 XHTML、[Polyglot HTML](http://www.w3.org/TR/html-polyglot/)，`DOCTYPE` 这几个字母需要大写。

HTML 和 XHTML 的 DOCTYPE 声明都有 strict/transitional/frameset 三种模式。
strict 模式禁止所有 presetational or deprecated elements（例如 font 标签）以及 frameset 标签；transitional 模式只禁止了 frameset 标签；frameset 模式与 transitional 模式相同，并且允许 frameset 标签。

[HTML 5 标准放弃了与 SGML 的兼容](http://www.w3.org/TR/html5-diff/#doctype)，所以其实不需要在文档开头引用 DTD，保留 DOCTYPE 是为了保证与旧浏览器的兼容。之所以选用 `<!DOCTYPE html>` 是因为[这个声明格式在当前所有的浏览器（IE、FF、Opera、Safar 等，即使没有实现 HTML 5）下都会以标准模式渲染](http://ejohn.org/blog/html5-doctype/)并且长度最短。

对于 XHTML 页面，只要 `Content-Type` 用了 `application/xhtml+xml` MIME 类型，就可以不声明 DOCTYPE。不过 IE 8- 不支持这个 `Content-Type` 取值，会被当成资源文件而弹出下载框，所以目前来说其实并没有什么用……

其他情况下，不声明 DOCTYPE 的话，浏览器会以 Quicks Mode 渲染页面。IE 9- 的 Quicks Mode 是指 IE 5.5 的渲染模式，不过 IE 10+ 和其他浏览器的 Quicks Mode 则是从 Almost Standards Mode 演化而来，WHATWG 有一个 [Quicks Mode 的标准文档](https://quirks.spec.whatwg.org/)。

更详细的信息可以参考这篇文章：[Activating Browser Modes with Doctype](https://hsivonen.fi/doctype/)。


### 常见的 meta 标签

可以参考 FEX 的[这篇文章](http://fex.baidu.com/blog/2014/10/html-head-tags/)，不过其中有部分已经过时了，比如 `viewport` 的 `minimal-ui` 属性在 iOS 8 中已经被去掉了


### HTML 语义化

[HTML5 Doctor](http://html5doctor.com/)


### Reflow and Repaint

参考[这篇文章](http://www.sitepoint.com/10-ways-minimize-reflows-improve-performance/)。

### LeetCode

LeetCode 地址为 [https://leetcode.com/](https://leetcode.com/)。

[《LeetCode 题解》](https://www.gitbook.com/book/siddontang/leetcode-solution/details) 这本电子书中有很详尽的 C++ 版本的题解。


### JavaScript 基本类型

根据 ES 2015 标准，JavaScript 的基本类型一共有 7 种，分别是 Undefined、Null、Boolean、String、Symbol、Number 以及 Object，其中 Symbol 是 ES 2015 标准中新增的基本类型。


### AJAX 跨域

[浅谈WEB跨域的实现（前端向）](http://www.cnblogs.com/vajoy/p/4295825.html)


### 服务器端推送

- [关于web通信技术](http://www.tony77.com/archives/431.html)


### absolute 和 float 的区别

两者都会脱离 normal flow（注意不要翻译成文档流），前者会覆盖 normal flow 中的元素，后者仍然占据位置


### 一小时之内写一个扫雷游戏

来源：[http://rkoutnik.com/articles/How-I-Interview.html](http://rkoutnik.com/articles/How-I-Interview.html)

思路/代码：[http://waitingfortheelevator.com/html-5-minesweeper-in-an-hour/](http://waitingfortheelevator.com/html-5-minesweeper-in-an-hour/)
