# 前端面试题总结

包括笔者本人遇到过的、网上见到过的以及自己想出来的各类前端相关的面试题。
主要适用于初中级前端（相当于阿里 P6 左右）。


部分参考文章如下：

- [Front-end Job Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions)
- [百度 FEX 团队面试题](https://github.com/fex-team/interview-questions)
- [阿里航旅事业部前端开发校招（电面）面试题](https://github.com/jayli/jayli.github.com/issues/19)
- [That JS Dude](http://thatjsdude.com/interview/index.html)
- [前端开发面试题](https://github.com/markyun/My-blog/tree/master/Front-end-Developer-Questions/Questions-and-Answers)
- [FE-Interview](https://github.com/qiu-deqing/FE-interview)
- [如何面试 JS 开发工程师](http://www.zhihu.com/question/37441607)

## 文章目录

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [HTML](#html)
  - [DOCTYPE 声明的作用、取值与区别](#doctype-%E5%A3%B0%E6%98%8E%E7%9A%84%E4%BD%9C%E7%94%A8%E3%80%81%E5%8F%96%E5%80%BC%E4%B8%8E%E5%8C%BA%E5%88%AB)
  - [常见的 meta 标签有哪些？移动端呢？](#%E5%B8%B8%E8%A7%81%E7%9A%84-meta-%E6%A0%87%E7%AD%BE%E6%9C%89%E5%93%AA%E4%BA%9B%EF%BC%9F%E7%A7%BB%E5%8A%A8%E7%AB%AF%E5%91%A2%EF%BC%9F)
  - [关于 HTML 语义化知道哪些？](#%E5%85%B3%E4%BA%8E-html-%E8%AF%AD%E4%B9%89%E5%8C%96%E7%9F%A5%E9%81%93%E5%93%AA%E4%BA%9B%EF%BC%9F)
  - [是否有关注 HTML 标准的演进？比较关注哪些方面？能否举一些例子？](#%E6%98%AF%E5%90%A6%E6%9C%89%E5%85%B3%E6%B3%A8-html-%E6%A0%87%E5%87%86%E7%9A%84%E6%BC%94%E8%BF%9B%EF%BC%9F%E6%AF%94%E8%BE%83%E5%85%B3%E6%B3%A8%E5%93%AA%E4%BA%9B%E6%96%B9%E9%9D%A2%EF%BC%9F%E8%83%BD%E5%90%A6%E4%B8%BE%E4%B8%80%E4%BA%9B%E4%BE%8B%E5%AD%90%EF%BC%9F)
- [CSS](#css)
  - [CSS 有几种引入方式？各自的优缺点？](#css-%E6%9C%89%E5%87%A0%E7%A7%8D%E5%BC%95%E5%85%A5%E6%96%B9%E5%BC%8F%EF%BC%9F%E5%90%84%E8%87%AA%E7%9A%84%E4%BC%98%E7%BC%BA%E7%82%B9%EF%BC%9F)
  - [不同浏览器上的默认样式，如何处理？（normalize/sanitize）](#%E4%B8%8D%E5%90%8C%E6%B5%8F%E8%A7%88%E5%99%A8%E4%B8%8A%E7%9A%84%E9%BB%98%E8%AE%A4%E6%A0%B7%E5%BC%8F%EF%BC%8C%E5%A6%82%E4%BD%95%E5%A4%84%E7%90%86%EF%BC%9F%EF%BC%88normalizesanitize%EF%BC%89)
  - [盒模型、IE 6/7 与现代浏览器的区别、如何兼容](#%E7%9B%92%E6%A8%A1%E5%9E%8B%E3%80%81ie-67-%E4%B8%8E%E7%8E%B0%E4%BB%A3%E6%B5%8F%E8%A7%88%E5%99%A8%E7%9A%84%E5%8C%BA%E5%88%AB%E3%80%81%E5%A6%82%E4%BD%95%E5%85%BC%E5%AE%B9)
  - [BFC 的概念](#bfc-%E7%9A%84%E6%A6%82%E5%BF%B5)
  - [containing block 和 stacking context 的概念和计算](#containing-block-%E5%92%8C-stacking-context-%E7%9A%84%E6%A6%82%E5%BF%B5%E5%92%8C%E8%AE%A1%E7%AE%97)
  - [position 和 display 各有几种取值？说说他们的含义与用途](#position-%E5%92%8C-display-%E5%90%84%E6%9C%89%E5%87%A0%E7%A7%8D%E5%8F%96%E5%80%BC%EF%BC%9F%E8%AF%B4%E8%AF%B4%E4%BB%96%E4%BB%AC%E7%9A%84%E5%90%AB%E4%B9%89%E4%B8%8E%E7%94%A8%E9%80%94)
  - [`position: absolute` 和 `float` 有什么区别](#position-absolute-%E5%92%8C-float-%E6%9C%89%E4%BB%80%E4%B9%88%E5%8C%BA%E5%88%AB)
  - [如何清除浮动？为什么要清除浮动？](#%E5%A6%82%E4%BD%95%E6%B8%85%E9%99%A4%E6%B5%AE%E5%8A%A8%EF%BC%9F%E4%B8%BA%E4%BB%80%E4%B9%88%E8%A6%81%E6%B8%85%E9%99%A4%E6%B5%AE%E5%8A%A8%EF%BC%9F)
  - [选择器相关问题](#%E9%80%89%E6%8B%A9%E5%99%A8%E7%9B%B8%E5%85%B3%E9%97%AE%E9%A2%98)
    - [specificity 的计算](#specificity-%E7%9A%84%E8%AE%A1%E7%AE%97)
    - [伪类和伪元素的区分](#%E4%BC%AA%E7%B1%BB%E5%92%8C%E4%BC%AA%E5%85%83%E7%B4%A0%E7%9A%84%E5%8C%BA%E5%88%86)
    - [选择器性能（浏览器如何进行匹配）](#%E9%80%89%E6%8B%A9%E5%99%A8%E6%80%A7%E8%83%BD%EF%BC%88%E6%B5%8F%E8%A7%88%E5%99%A8%E5%A6%82%E4%BD%95%E8%BF%9B%E8%A1%8C%E5%8C%B9%E9%85%8D%EF%BC%89)
    - [CSS3 和 CSS4 选择器知道哪些](#css3-%E5%92%8C-css4-%E9%80%89%E6%8B%A9%E5%99%A8%E7%9F%A5%E9%81%93%E5%93%AA%E4%BA%9B)
  - [CSS 优化](#css-%E4%BC%98%E5%8C%96)
    - [网络加载方面有哪些手段](#%E7%BD%91%E7%BB%9C%E5%8A%A0%E8%BD%BD%E6%96%B9%E9%9D%A2%E6%9C%89%E5%93%AA%E4%BA%9B%E6%89%8B%E6%AE%B5)
    - [渲染性能的方面呢](#%E6%B8%B2%E6%9F%93%E6%80%A7%E8%83%BD%E7%9A%84%E6%96%B9%E9%9D%A2%E5%91%A2)
  - [用过哪些 CSS 方面的工具](#%E7%94%A8%E8%BF%87%E5%93%AA%E4%BA%9B-css-%E6%96%B9%E9%9D%A2%E7%9A%84%E5%B7%A5%E5%85%B7)
  - [随便谈谈 CSS 工程化](#%E9%9A%8F%E4%BE%BF%E8%B0%88%E8%B0%88-css-%E5%B7%A5%E7%A8%8B%E5%8C%96)
- [JavaScript](#javascript)
  - [JavaScript 有哪些基本类型](#javascript-%E6%9C%89%E5%93%AA%E4%BA%9B%E5%9F%BA%E6%9C%AC%E7%B1%BB%E5%9E%8B)
  - [区分不同类型的方法有哪些，各有什么问题](#%E5%8C%BA%E5%88%86%E4%B8%8D%E5%90%8C%E7%B1%BB%E5%9E%8B%E7%9A%84%E6%96%B9%E6%B3%95%E6%9C%89%E5%93%AA%E4%BA%9B%EF%BC%8C%E5%90%84%E6%9C%89%E4%BB%80%E4%B9%88%E9%97%AE%E9%A2%98)
  - [闭包的概念 & 用途](#%E9%97%AD%E5%8C%85%E7%9A%84%E6%A6%82%E5%BF%B5-&-%E7%94%A8%E9%80%94)
  - [`apply` 和 `call` 的用途和区别](#apply-%E5%92%8C-call-%E7%9A%84%E7%94%A8%E9%80%94%E5%92%8C%E5%8C%BA%E5%88%AB)
  - [原型继承的概念， `prototype` 和 `__proto__` 的区别](#%E5%8E%9F%E5%9E%8B%E7%BB%A7%E6%89%BF%E7%9A%84%E6%A6%82%E5%BF%B5%EF%BC%8C-prototype-%E5%92%8C-__proto__-%E7%9A%84%E5%8C%BA%E5%88%AB)
  - [JavaScript 如何实现继承？对象的几种创建方式？](#javascript-%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E7%BB%A7%E6%89%BF%EF%BC%9F%E5%AF%B9%E8%B1%A1%E7%9A%84%E5%87%A0%E7%A7%8D%E5%88%9B%E5%BB%BA%E6%96%B9%E5%BC%8F%EF%BC%9F)
  - [是否碰到过内存泄露？能否说一下引起内存泄露的常见原因（网上大部分文章都是跟 IE 相关的，其实没什么必要了解，闭包方面有必要知道）？有什么工具可以调试？](#%E6%98%AF%E5%90%A6%E7%A2%B0%E5%88%B0%E8%BF%87%E5%86%85%E5%AD%98%E6%B3%84%E9%9C%B2%EF%BC%9F%E8%83%BD%E5%90%A6%E8%AF%B4%E4%B8%80%E4%B8%8B%E5%BC%95%E8%B5%B7%E5%86%85%E5%AD%98%E6%B3%84%E9%9C%B2%E7%9A%84%E5%B8%B8%E8%A7%81%E5%8E%9F%E5%9B%A0%EF%BC%88%E7%BD%91%E4%B8%8A%E5%A4%A7%E9%83%A8%E5%88%86%E6%96%87%E7%AB%A0%E9%83%BD%E6%98%AF%E8%B7%9F-ie-%E7%9B%B8%E5%85%B3%E7%9A%84%EF%BC%8C%E5%85%B6%E5%AE%9E%E6%B2%A1%E4%BB%80%E4%B9%88%E5%BF%85%E8%A6%81%E4%BA%86%E8%A7%A3%EF%BC%8C%E9%97%AD%E5%8C%85%E6%96%B9%E9%9D%A2%E6%9C%89%E5%BF%85%E8%A6%81%E7%9F%A5%E9%81%93%EF%BC%89%EF%BC%9F%E6%9C%89%E4%BB%80%E4%B9%88%E5%B7%A5%E5%85%B7%E5%8F%AF%E4%BB%A5%E8%B0%83%E8%AF%95%EF%BC%9F)
  - [JavaScript 设计模式知道哪些？Proxy 模式怎么用？](#javascript-%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F%E7%9F%A5%E9%81%93%E5%93%AA%E4%BA%9B%EF%BC%9Fproxy-%E6%A8%A1%E5%BC%8F%E6%80%8E%E4%B9%88%E7%94%A8%EF%BC%9F)
  - [ES6 是否有了解](#es6-%E6%98%AF%E5%90%A6%E6%9C%89%E4%BA%86%E8%A7%A3)
  - [JavaScript 模块化（常见规范、工具、实现原理）](#javascript-%E6%A8%A1%E5%9D%97%E5%8C%96%EF%BC%88%E5%B8%B8%E8%A7%81%E8%A7%84%E8%8C%83%E3%80%81%E5%B7%A5%E5%85%B7%E3%80%81%E5%AE%9E%E7%8E%B0%E5%8E%9F%E7%90%86%EF%BC%89)
- [DOM](#dom)
  - [DOM 的事件机制](#dom-%E7%9A%84%E4%BA%8B%E4%BB%B6%E6%9C%BA%E5%88%B6)
    - [冒泡与捕获的概念，如何阻止冒泡](#%E5%86%92%E6%B3%A1%E4%B8%8E%E6%8D%95%E8%8E%B7%E7%9A%84%E6%A6%82%E5%BF%B5%EF%BC%8C%E5%A6%82%E4%BD%95%E9%98%BB%E6%AD%A2%E5%86%92%E6%B3%A1)
    - [Delegation](#delegation)
    - [鼠标点击 a 标签其中会有多少个时间产生](#%E9%BC%A0%E6%A0%87%E7%82%B9%E5%87%BB-a-%E6%A0%87%E7%AD%BE%E5%85%B6%E4%B8%AD%E4%BC%9A%E6%9C%89%E5%A4%9A%E5%B0%91%E4%B8%AA%E6%97%B6%E9%97%B4%E4%BA%A7%E7%94%9F)
    - [如何区分 dbclick 和 click](#%E5%A6%82%E4%BD%95%E5%8C%BA%E5%88%86-dbclick-%E5%92%8C-click)
  - [ajax 请求中 readyState 有哪些状态（这个问题我感觉太不常考了……但既然见到过那就收录进来了）](#ajax-%E8%AF%B7%E6%B1%82%E4%B8%AD-readystate-%E6%9C%89%E5%93%AA%E4%BA%9B%E7%8A%B6%E6%80%81%EF%BC%88%E8%BF%99%E4%B8%AA%E9%97%AE%E9%A2%98%E6%88%91%E6%84%9F%E8%A7%89%E5%A4%AA%E4%B8%8D%E5%B8%B8%E8%80%83%E4%BA%86%E2%80%A6%E2%80%A6%E4%BD%86%E6%97%A2%E7%84%B6%E8%A7%81%E5%88%B0%E8%BF%87%E9%82%A3%E5%B0%B1%E6%94%B6%E5%BD%95%E8%BF%9B%E6%9D%A5%E4%BA%86%EF%BC%89)
  - [ajax 跨域](#ajax-%E8%B7%A8%E5%9F%9F)
    - [怎样算是跨域？](#%E6%80%8E%E6%A0%B7%E7%AE%97%E6%98%AF%E8%B7%A8%E5%9F%9F%EF%BC%9F)
    - [跨域的方法有哪些？实现原理是什么？兼容性如何？各自有什么缺点？](#%E8%B7%A8%E5%9F%9F%E7%9A%84%E6%96%B9%E6%B3%95%E6%9C%89%E5%93%AA%E4%BA%9B%EF%BC%9F%E5%AE%9E%E7%8E%B0%E5%8E%9F%E7%90%86%E6%98%AF%E4%BB%80%E4%B9%88%EF%BC%9F%E5%85%BC%E5%AE%B9%E6%80%A7%E5%A6%82%E4%BD%95%EF%BC%9F%E5%90%84%E8%87%AA%E6%9C%89%E4%BB%80%E4%B9%88%E7%BC%BA%E7%82%B9%EF%BC%9F)
    - [JSONP 如果页面编码和被请求的资源编码不一致如何处理](#jsonp-%E5%A6%82%E6%9E%9C%E9%A1%B5%E9%9D%A2%E7%BC%96%E7%A0%81%E5%92%8C%E8%A2%AB%E8%AF%B7%E6%B1%82%E7%9A%84%E8%B5%84%E6%BA%90%E7%BC%96%E7%A0%81%E4%B8%8D%E4%B8%80%E8%87%B4%E5%A6%82%E4%BD%95%E5%A4%84%E7%90%86)
  - [服务器端消息推送有哪些方法？实现原理？兼容性？缺点？](#%E6%9C%8D%E5%8A%A1%E5%99%A8%E7%AB%AF%E6%B6%88%E6%81%AF%E6%8E%A8%E9%80%81%E6%9C%89%E5%93%AA%E4%BA%9B%E6%96%B9%E6%B3%95%EF%BC%9F%E5%AE%9E%E7%8E%B0%E5%8E%9F%E7%90%86%EF%BC%9F%E5%85%BC%E5%AE%B9%E6%80%A7%EF%BC%9F%E7%BC%BA%E7%82%B9%EF%BC%9F)
  - [jQuery.ready() 实际上是 DOM 中的什么事件？](#jqueryready-%E5%AE%9E%E9%99%85%E4%B8%8A%E6%98%AF-dom-%E4%B8%AD%E7%9A%84%E4%BB%80%E4%B9%88%E4%BA%8B%E4%BB%B6%EF%BC%9F)
  - [`window.onload` 和 `$.ready()` 事件有什么区别？](#windowonload-%E5%92%8C-ready-%E4%BA%8B%E4%BB%B6%E6%9C%89%E4%BB%80%E4%B9%88%E5%8C%BA%E5%88%AB%EF%BC%9F)
- [前端性能优化](#%E5%89%8D%E7%AB%AF%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96)
  - [雅虎 24 条，说出越多越好](#%E9%9B%85%E8%99%8E-24-%E6%9D%A1%EF%BC%8C%E8%AF%B4%E5%87%BA%E8%B6%8A%E5%A4%9A%E8%B6%8A%E5%A5%BD)
  - [是否有其他性能优化的经验？](#%E6%98%AF%E5%90%A6%E6%9C%89%E5%85%B6%E4%BB%96%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96%E7%9A%84%E7%BB%8F%E9%AA%8C%EF%BC%9F)
- [页面性能分析](#%E9%A1%B5%E9%9D%A2%E6%80%A7%E8%83%BD%E5%88%86%E6%9E%90)
  - [页面性能一般可以有哪些指标](#%E9%A1%B5%E9%9D%A2%E6%80%A7%E8%83%BD%E4%B8%80%E8%88%AC%E5%8F%AF%E4%BB%A5%E6%9C%89%E5%93%AA%E4%BA%9B%E6%8C%87%E6%A0%87)
  - [页面性能记录和分析有哪些方法？除了常见的那些方法之外在现代浏览器里还有其他什么新手段吗？](#%E9%A1%B5%E9%9D%A2%E6%80%A7%E8%83%BD%E8%AE%B0%E5%BD%95%E5%92%8C%E5%88%86%E6%9E%90%E6%9C%89%E5%93%AA%E4%BA%9B%E6%96%B9%E6%B3%95%EF%BC%9F%E9%99%A4%E4%BA%86%E5%B8%B8%E8%A7%81%E7%9A%84%E9%82%A3%E4%BA%9B%E6%96%B9%E6%B3%95%E4%B9%8B%E5%A4%96%E5%9C%A8%E7%8E%B0%E4%BB%A3%E6%B5%8F%E8%A7%88%E5%99%A8%E9%87%8C%E8%BF%98%E6%9C%89%E5%85%B6%E4%BB%96%E4%BB%80%E4%B9%88%E6%96%B0%E6%89%8B%E6%AE%B5%E5%90%97%EF%BC%9F)
  - [用过什么性能分析的工具](#%E7%94%A8%E8%BF%87%E4%BB%80%E4%B9%88%E6%80%A7%E8%83%BD%E5%88%86%E6%9E%90%E7%9A%84%E5%B7%A5%E5%85%B7)
- [前端安全](#%E5%89%8D%E7%AB%AF%E5%AE%89%E5%85%A8)
  - [XSS 的概念、知道哪些解决办法（常规的就行，不必太深入）](#xss-%E7%9A%84%E6%A6%82%E5%BF%B5%E3%80%81%E7%9F%A5%E9%81%93%E5%93%AA%E4%BA%9B%E8%A7%A3%E5%86%B3%E5%8A%9E%E6%B3%95%EF%BC%88%E5%B8%B8%E8%A7%84%E7%9A%84%E5%B0%B1%E8%A1%8C%EF%BC%8C%E4%B8%8D%E5%BF%85%E5%A4%AA%E6%B7%B1%E5%85%A5%EF%BC%89)
  - [`escape` / `encodeURI` / `encodeURIComponent` 的区别](#escape--encodeuri--encodeuricomponent-%E7%9A%84%E5%8C%BA%E5%88%AB)
  - [CSRF 攻击的概念、防御手段](#csrf-%E6%94%BB%E5%87%BB%E7%9A%84%E6%A6%82%E5%BF%B5%E3%80%81%E9%98%B2%E5%BE%A1%E6%89%8B%E6%AE%B5)
  - [CSP](#csp)
  - [淘宝店铺装修的 CSS 过滤、JS 过滤有什么思路](#%E6%B7%98%E5%AE%9D%E5%BA%97%E9%93%BA%E8%A3%85%E4%BF%AE%E7%9A%84-css-%E8%BF%87%E6%BB%A4%E3%80%81js-%E8%BF%87%E6%BB%A4%E6%9C%89%E4%BB%80%E4%B9%88%E6%80%9D%E8%B7%AF)
  - [代码质量](#%E4%BB%A3%E7%A0%81%E8%B4%A8%E9%87%8F)
- [后端](#%E5%90%8E%E7%AB%AF)
  - [讲讲 session 的实现原理，cookies 和 session 的关系，客户端禁用 cookies 后怎么使用 session？](#%E8%AE%B2%E8%AE%B2-session-%E7%9A%84%E5%AE%9E%E7%8E%B0%E5%8E%9F%E7%90%86%EF%BC%8Ccookies-%E5%92%8C-session-%E7%9A%84%E5%85%B3%E7%B3%BB%EF%BC%8C%E5%AE%A2%E6%88%B7%E7%AB%AF%E7%A6%81%E7%94%A8-cookies-%E5%90%8E%E6%80%8E%E4%B9%88%E4%BD%BF%E7%94%A8-session%EF%BC%9F)
  - [多台服务器之间该如何共享 session](#%E5%A4%9A%E5%8F%B0%E6%9C%8D%E5%8A%A1%E5%99%A8%E4%B9%8B%E9%97%B4%E8%AF%A5%E5%A6%82%E4%BD%95%E5%85%B1%E4%BA%AB-session)
  - [讲讲 RESTful](#%E8%AE%B2%E8%AE%B2-restful)
- [NodeJS](#nodejs)
  - [callback hell 以及目前的解决方案](#callback-hell-%E4%BB%A5%E5%8F%8A%E7%9B%AE%E5%89%8D%E7%9A%84%E8%A7%A3%E5%86%B3%E6%96%B9%E6%A1%88)
  - [用过 koa 吗？thunk 是什么？（等 koa 2 正式版出来以后这个可以不用问了）](#%E7%94%A8%E8%BF%87-koa-%E5%90%97%EF%BC%9Fthunk-%E6%98%AF%E4%BB%80%E4%B9%88%EF%BC%9F%EF%BC%88%E7%AD%89-koa-2-%E6%AD%A3%E5%BC%8F%E7%89%88%E5%87%BA%E6%9D%A5%E4%BB%A5%E5%90%8E%E8%BF%99%E4%B8%AA%E5%8F%AF%E4%BB%A5%E4%B8%8D%E7%94%A8%E9%97%AE%E4%BA%86%EF%BC%89)
  - [什么是事件循环？Node 中有哪些类型的函数/调用是异步的？哪些是同步的？](#%E4%BB%80%E4%B9%88%E6%98%AF%E4%BA%8B%E4%BB%B6%E5%BE%AA%E7%8E%AF%EF%BC%9Fnode-%E4%B8%AD%E6%9C%89%E5%93%AA%E4%BA%9B%E7%B1%BB%E5%9E%8B%E7%9A%84%E5%87%BD%E6%95%B0%E8%B0%83%E7%94%A8%E6%98%AF%E5%BC%82%E6%AD%A5%E7%9A%84%EF%BC%9F%E5%93%AA%E4%BA%9B%E6%98%AF%E5%90%8C%E6%AD%A5%E7%9A%84%EF%BC%9F)
  - [怎样绑定 Node 程序到 80 端口[#绑定-node-程序到-80-端口]？](#%E6%80%8E%E6%A0%B7%E7%BB%91%E5%AE%9A-node-%E7%A8%8B%E5%BA%8F%E5%88%B0-80-%E7%AB%AF%E5%8F%A3%E7%BB%91%E5%AE%9A-node-%E7%A8%8B%E5%BA%8F%E5%88%B0-80-%E7%AB%AF%E5%8F%A3%EF%BC%9F)
  - [有哪些方法可以让 Node 程序遇到错误后自动重启](#%E6%9C%89%E5%93%AA%E4%BA%9B%E6%96%B9%E6%B3%95%E5%8F%AF%E4%BB%A5%E8%AE%A9-node-%E7%A8%8B%E5%BA%8F%E9%81%87%E5%88%B0%E9%94%99%E8%AF%AF%E5%90%8E%E8%87%AA%E5%8A%A8%E9%87%8D%E5%90%AF)
  - [如何实现一个 writable stream？](#%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E4%B8%80%E4%B8%AA-writable-stream%EF%BC%9F)
  - [Node.js 中怎么删文件？](#nodejs-%E4%B8%AD%E6%80%8E%E4%B9%88%E5%88%A0%E6%96%87%E4%BB%B6%EF%BC%9F)
  - [在 Node 中直接用 MySQL 的话，客户端一定时间没有活动的话 MySQL 会断开连接，一般怎么处理这个问题？](#%E5%9C%A8-node-%E4%B8%AD%E7%9B%B4%E6%8E%A5%E7%94%A8-mysql-%E7%9A%84%E8%AF%9D%EF%BC%8C%E5%AE%A2%E6%88%B7%E7%AB%AF%E4%B8%80%E5%AE%9A%E6%97%B6%E9%97%B4%E6%B2%A1%E6%9C%89%E6%B4%BB%E5%8A%A8%E7%9A%84%E8%AF%9D-mysql-%E4%BC%9A%E6%96%AD%E5%BC%80%E8%BF%9E%E6%8E%A5%EF%BC%8C%E4%B8%80%E8%88%AC%E6%80%8E%E4%B9%88%E5%A4%84%E7%90%86%E8%BF%99%E4%B8%AA%E9%97%AE%E9%A2%98%EF%BC%9F)
- [TypeScript](#typescript)
  - [都说 TypeScript 的类型系统是 unsound 的，请问这个 unsound 是什么意思？具体表现在什么地方？](#%E9%83%BD%E8%AF%B4-typescript-%E7%9A%84%E7%B1%BB%E5%9E%8B%E7%B3%BB%E7%BB%9F%E6%98%AF-unsound-%E7%9A%84%EF%BC%8C%E8%AF%B7%E9%97%AE%E8%BF%99%E4%B8%AA-unsound-%E6%98%AF%E4%BB%80%E4%B9%88%E6%84%8F%E6%80%9D%EF%BC%9F%E5%85%B7%E4%BD%93%E8%A1%A8%E7%8E%B0%E5%9C%A8%E4%BB%80%E4%B9%88%E5%9C%B0%E6%96%B9%EF%BC%9F)
  - [`interface` 和 `declare class` 都可以用来描述一个类，请问这两者的区别是什么？](#interface-%E5%92%8C-declare-class-%E9%83%BD%E5%8F%AF%E4%BB%A5%E7%94%A8%E6%9D%A5%E6%8F%8F%E8%BF%B0%E4%B8%80%E4%B8%AA%E7%B1%BB%EF%BC%8C%E8%AF%B7%E9%97%AE%E8%BF%99%E4%B8%A4%E8%80%85%E7%9A%84%E5%8C%BA%E5%88%AB%E6%98%AF%E4%BB%80%E4%B9%88%EF%BC%9F)
- [网络](#%E7%BD%91%E7%BB%9C)
  - [TCP 三次握手](#tcp-%E4%B8%89%E6%AC%A1%E6%8F%A1%E6%89%8B)
    - [具体过程](#%E5%85%B7%E4%BD%93%E8%BF%87%E7%A8%8B)
    - [为什么要这么设计](#%E4%B8%BA%E4%BB%80%E4%B9%88%E8%A6%81%E8%BF%99%E4%B9%88%E8%AE%BE%E8%AE%A1)
  - [说一下网络五层模型（HTTP 协议从应用层到底层都基于哪些协议），HTTP 协议头字段说上来几个，缓存字段是怎么定义的，http 和 https 的区别，在具体使用的时候有什么不一样。是否尽可能详细的掌握 HTTP 协议](#%E8%AF%B4%E4%B8%80%E4%B8%8B%E7%BD%91%E7%BB%9C%E4%BA%94%E5%B1%82%E6%A8%A1%E5%9E%8B%EF%BC%88http-%E5%8D%8F%E8%AE%AE%E4%BB%8E%E5%BA%94%E7%94%A8%E5%B1%82%E5%88%B0%E5%BA%95%E5%B1%82%E9%83%BD%E5%9F%BA%E4%BA%8E%E5%93%AA%E4%BA%9B%E5%8D%8F%E8%AE%AE%EF%BC%89%EF%BC%8Chttp-%E5%8D%8F%E8%AE%AE%E5%A4%B4%E5%AD%97%E6%AE%B5%E8%AF%B4%E4%B8%8A%E6%9D%A5%E5%87%A0%E4%B8%AA%EF%BC%8C%E7%BC%93%E5%AD%98%E5%AD%97%E6%AE%B5%E6%98%AF%E6%80%8E%E4%B9%88%E5%AE%9A%E4%B9%89%E7%9A%84%EF%BC%8Chttp-%E5%92%8C-https-%E7%9A%84%E5%8C%BA%E5%88%AB%EF%BC%8C%E5%9C%A8%E5%85%B7%E4%BD%93%E4%BD%BF%E7%94%A8%E7%9A%84%E6%97%B6%E5%80%99%E6%9C%89%E4%BB%80%E4%B9%88%E4%B8%8D%E4%B8%80%E6%A0%B7%E3%80%82%E6%98%AF%E5%90%A6%E5%B0%BD%E5%8F%AF%E8%83%BD%E8%AF%A6%E7%BB%86%E7%9A%84%E6%8E%8C%E6%8F%A1-http-%E5%8D%8F%E8%AE%AE)
  - [HTTP 状态码](#http-%E7%8A%B6%E6%80%81%E7%A0%81)
    - [1、2、3、4、5 开头分别表示什么](#1%E3%80%812%E3%80%813%E3%80%814%E3%80%815-%E5%BC%80%E5%A4%B4%E5%88%86%E5%88%AB%E8%A1%A8%E7%A4%BA%E4%BB%80%E4%B9%88)
    - [301 和 302 的区别、为什么要区分](#301-%E5%92%8C-302-%E7%9A%84%E5%8C%BA%E5%88%AB%E3%80%81%E4%B8%BA%E4%BB%80%E4%B9%88%E8%A6%81%E5%8C%BA%E5%88%86)
    - [304 表示什么](#304-%E8%A1%A8%E7%A4%BA%E4%BB%80%E4%B9%88)
  - [如何防止 304](#%E5%A6%82%E4%BD%95%E9%98%B2%E6%AD%A2-304)
  - [`keep-alive`](#keep-alive)
  - [cookies 是干嘛的，服务器和浏览器之间的 cookies 是怎么传的，httponly 的 cookies 和可读写的 cookie 有什么区别，有无长度限制，cookies 被禁用后可以考虑用什么替代](#cookies-%E6%98%AF%E5%B9%B2%E5%98%9B%E7%9A%84%EF%BC%8C%E6%9C%8D%E5%8A%A1%E5%99%A8%E5%92%8C%E6%B5%8F%E8%A7%88%E5%99%A8%E4%B9%8B%E9%97%B4%E7%9A%84-cookies-%E6%98%AF%E6%80%8E%E4%B9%88%E4%BC%A0%E7%9A%84%EF%BC%8Chttponly-%E7%9A%84-cookies-%E5%92%8C%E5%8F%AF%E8%AF%BB%E5%86%99%E7%9A%84-cookie-%E6%9C%89%E4%BB%80%E4%B9%88%E5%8C%BA%E5%88%AB%EF%BC%8C%E6%9C%89%E6%97%A0%E9%95%BF%E5%BA%A6%E9%99%90%E5%88%B6%EF%BC%8Ccookies-%E8%A2%AB%E7%A6%81%E7%94%A8%E5%90%8E%E5%8F%AF%E4%BB%A5%E8%80%83%E8%99%91%E7%94%A8%E4%BB%80%E4%B9%88%E6%9B%BF%E4%BB%A3)
  - [GET/POST 区别](#getpost-%E5%8C%BA%E5%88%AB)
  - [一个页面从输入 URL 到页面加载完的过程中都发生了什么事情？越详细越好](#%E4%B8%80%E4%B8%AA%E9%A1%B5%E9%9D%A2%E4%BB%8E%E8%BE%93%E5%85%A5-url-%E5%88%B0%E9%A1%B5%E9%9D%A2%E5%8A%A0%E8%BD%BD%E5%AE%8C%E7%9A%84%E8%BF%87%E7%A8%8B%E4%B8%AD%E9%83%BD%E5%8F%91%E7%94%9F%E4%BA%86%E4%BB%80%E4%B9%88%E4%BA%8B%E6%83%85%EF%BC%9F%E8%B6%8A%E8%AF%A6%E7%BB%86%E8%B6%8A%E5%A5%BD)
  - [关于 HTTP2 知道哪些？对未来前端开发可能会有哪些影响？](#%E5%85%B3%E4%BA%8E-http2-%E7%9F%A5%E9%81%93%E5%93%AA%E4%BA%9B%EF%BC%9F%E5%AF%B9%E6%9C%AA%E6%9D%A5%E5%89%8D%E7%AB%AF%E5%BC%80%E5%8F%91%E5%8F%AF%E8%83%BD%E4%BC%9A%E6%9C%89%E5%93%AA%E4%BA%9B%E5%BD%B1%E5%93%8D%EF%BC%9F)
- [其他](#%E5%85%B6%E4%BB%96)
  - [会不会用 ps 扣图，png、jpg、gif 这些图片格式解释一下，分别什么时候用。是否了解webp](#%E4%BC%9A%E4%B8%8D%E4%BC%9A%E7%94%A8-ps-%E6%89%A3%E5%9B%BE%EF%BC%8Cpng%E3%80%81jpg%E3%80%81gif-%E8%BF%99%E4%BA%9B%E5%9B%BE%E7%89%87%E6%A0%BC%E5%BC%8F%E8%A7%A3%E9%87%8A%E4%B8%80%E4%B8%8B%EF%BC%8C%E5%88%86%E5%88%AB%E4%BB%80%E4%B9%88%E6%97%B6%E5%80%99%E7%94%A8%E3%80%82%E6%98%AF%E5%90%A6%E4%BA%86%E8%A7%A3webp)
  - [是否了解开源的工具 bower、npm、yeoman、grunt、gulp、webpack，有无用过，有无写过，一个 npm 的包里的 package.json 具备的必要的字段都有哪些（名称、版本号，依赖）](#%E6%98%AF%E5%90%A6%E4%BA%86%E8%A7%A3%E5%BC%80%E6%BA%90%E7%9A%84%E5%B7%A5%E5%85%B7-bower%E3%80%81npm%E3%80%81yeoman%E3%80%81grunt%E3%80%81gulp%E3%80%81webpack%EF%BC%8C%E6%9C%89%E6%97%A0%E7%94%A8%E8%BF%87%EF%BC%8C%E6%9C%89%E6%97%A0%E5%86%99%E8%BF%87%EF%BC%8C%E4%B8%80%E4%B8%AA-npm-%E7%9A%84%E5%8C%85%E9%87%8C%E7%9A%84-packagejson-%E5%85%B7%E5%A4%87%E7%9A%84%E5%BF%85%E8%A6%81%E7%9A%84%E5%AD%97%E6%AE%B5%E9%83%BD%E6%9C%89%E5%93%AA%E4%BA%9B%EF%BC%88%E5%90%8D%E7%A7%B0%E3%80%81%E7%89%88%E6%9C%AC%E5%8F%B7%EF%BC%8C%E4%BE%9D%E8%B5%96%EF%BC%89)
- [手写代码](#%E6%89%8B%E5%86%99%E4%BB%A3%E7%A0%81)
  - [walkTheDOM 函数，从 `<body>` 标签起，遍历所有节点并打印标签名](#walkthedom-%E5%87%BD%E6%95%B0%EF%BC%8C%E4%BB%8E-body-%E6%A0%87%E7%AD%BE%E8%B5%B7%EF%BC%8C%E9%81%8D%E5%8E%86%E6%89%80%E6%9C%89%E8%8A%82%E7%82%B9%E5%B9%B6%E6%89%93%E5%8D%B0%E6%A0%87%E7%AD%BE%E5%90%8D)
  - [addClass](#addclass)
  - [实现一个简单的 pub-sub 库](#%E5%AE%9E%E7%8E%B0%E4%B8%80%E4%B8%AA%E7%AE%80%E5%8D%95%E7%9A%84-pub-sub-%E5%BA%93)
  - [实现 `_.flatten()`](#%E5%AE%9E%E7%8E%B0-_flatten)
  - [object deep clone](#object-deep-clone)
  - [isPrime](#isprime)
  - [quick sort](#quick-sort)
  - [merge sort](#merge-sort)
  - [binary search](#binary-search)
  - [throttle & debounce](#throttle-&-debounce)
  - [实现 `Object.create()`（不用完全遵循标准，实现蝴蝶书上的版本就够了）](#%E5%AE%9E%E7%8E%B0-objectcreate%EF%BC%88%E4%B8%8D%E7%94%A8%E5%AE%8C%E5%85%A8%E9%81%B5%E5%BE%AA%E6%A0%87%E5%87%86%EF%BC%8C%E5%AE%9E%E7%8E%B0%E8%9D%B4%E8%9D%B6%E4%B9%A6%E4%B8%8A%E7%9A%84%E7%89%88%E6%9C%AC%E5%B0%B1%E5%A4%9F%E4%BA%86%EF%BC%89)
  - [`Function.prototype.bind`](#functionprototypebind)
  - [CSS 实现元素的水平垂直居中](#css-%E5%AE%9E%E7%8E%B0%E5%85%83%E7%B4%A0%E7%9A%84%E6%B0%B4%E5%B9%B3%E5%9E%82%E7%9B%B4%E5%B1%85%E4%B8%AD)
  - [实现一个圣杯布局](#%E5%AE%9E%E7%8E%B0%E4%B8%80%E4%B8%AA%E5%9C%A3%E6%9D%AF%E5%B8%83%E5%B1%80)
  - [carousel 组件](#carousel-%E7%BB%84%E4%BB%B6)
  - [自动补全组件](#%E8%87%AA%E5%8A%A8%E8%A1%A5%E5%85%A8%E7%BB%84%E4%BB%B6)
  - [overlay 组件](#overlay-%E7%BB%84%E4%BB%B6)
  - [popup 组件](#popup-%E7%BB%84%E4%BB%B6)
  - [drag & drop 组件，分别用 jQuery、MVVM、React 和 RxJS 实现一遍](#drag-&-drop-%E7%BB%84%E4%BB%B6%EF%BC%8C%E5%88%86%E5%88%AB%E7%94%A8-jquery%E3%80%81mvvm%E3%80%81react-%E5%92%8C-rxjs-%E5%AE%9E%E7%8E%B0%E4%B8%80%E9%81%8D)
  - [一小时之内写一个扫雷游戏](#%E4%B8%80%E5%B0%8F%E6%97%B6%E4%B9%8B%E5%86%85%E5%86%99%E4%B8%80%E4%B8%AA%E6%89%AB%E9%9B%B7%E6%B8%B8%E6%88%8F)
- [代码实现思路](#%E4%BB%A3%E7%A0%81%E5%AE%9E%E7%8E%B0%E6%80%9D%E8%B7%AF)
  - [如果要你实现一个 AMD 加载器，你将如何实现？讲一下思路和需要注意的点，最好有伪代码](#%E5%A6%82%E6%9E%9C%E8%A6%81%E4%BD%A0%E5%AE%9E%E7%8E%B0%E4%B8%80%E4%B8%AA-amd-%E5%8A%A0%E8%BD%BD%E5%99%A8%EF%BC%8C%E4%BD%A0%E5%B0%86%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%EF%BC%9F%E8%AE%B2%E4%B8%80%E4%B8%8B%E6%80%9D%E8%B7%AF%E5%92%8C%E9%9C%80%E8%A6%81%E6%B3%A8%E6%84%8F%E7%9A%84%E7%82%B9%EF%BC%8C%E6%9C%80%E5%A5%BD%E6%9C%89%E4%BC%AA%E4%BB%A3%E7%A0%81)
  - [Sizzles （jQuery 的选择器模块）的实现思路](#sizzles-%EF%BC%88jquery-%E7%9A%84%E9%80%89%E6%8B%A9%E5%99%A8%E6%A8%A1%E5%9D%97%EF%BC%89%E7%9A%84%E5%AE%9E%E7%8E%B0%E6%80%9D%E8%B7%AF)
- [算法题](#%E7%AE%97%E6%B3%95%E9%A2%98)
  - [topK](#topk)
  - [翻转单链表](#%E7%BF%BB%E8%BD%AC%E5%8D%95%E9%93%BE%E8%A1%A8)
  - [反转二叉树](#%E5%8F%8D%E8%BD%AC%E4%BA%8C%E5%8F%89%E6%A0%91)
  - [单向列表判断是否有环](#%E5%8D%95%E5%90%91%E5%88%97%E8%A1%A8%E5%88%A4%E6%96%AD%E6%98%AF%E5%90%A6%E6%9C%89%E7%8E%AF)
  - [LeetCode](#leetcode)
  - [careercup](#careercup)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## HTML

### DOCTYPE 声明的作用、取值与区别

[HTML 4.01 和 XHTML 都基于 SMGL](http://www.w3.org/TR/REC-html40/intro/sgmltut.html)，所以需要在文档开头声明引用一个 DTD。

在 HTML 5 中，DOCTYPE 不区分大小写；不过对于 XHTML、[Polyglot HTML](http://www.w3.org/TR/html-polyglot/)，`DOCTYPE` 这几个字母需要大写。

HTML 和 XHTML 的 DOCTYPE 声明都有 strict/transitional/frameset 三种模式。
strict 模式禁止所有 presetational or deprecated elements（例如 font 标签）以及 frameset 标签；transitional 模式只禁止了 frameset 标签；frameset 模式与 transitional 模式相同，并且允许 frameset 标签。

[HTML 5 标准放弃了与 SGML 的兼容](http://www.w3.org/TR/html5-diff/#doctype)，所以其实不需要在文档开头引用 DTD，保留 DOCTYPE 是为了保证与旧浏览器的兼容。之所以选用 `<!DOCTYPE html>` 是因为[这个声明格式在当前所有的浏览器（IE、FF、Opera、Safar 等，即使没有实现 HTML 5）下都会以标准模式渲染](http://ejohn.org/blog/html5-doctype/)并且长度最短。

对于 XHTML 页面，只要 `Content-Type` 用了 `application/xhtml+xml` MIME 类型，就可以不声明 DOCTYPE。不过 IE 8- 不支持这个 `Content-Type` 取值，会被当成资源文件而弹出下载框，所以目前来说其实并没有什么用……

其他情况下，不声明 DOCTYPE 的话，浏览器会以 Quicks Mode 渲染页面。IE 9- 的 Quicks Mode 是指 IE 5.5 的渲染模式，不过 IE 10+ 和其他浏览器的 Quicks Mode 则是从 Almost Standards Mode 演化而来，WHATWG 有一个 [Quicks Mode 的标准文档](https://quirks.spec.whatwg.org/)。

更详细的信息可以参考这篇文章：[Activating Browser Modes with Doctype](https://hsivonen.fi/doctype/)。

### 常见的 meta 标签有哪些？移动端呢？

- [常用的 HTML 头部标签](https://github.com/yisibl/blog/issues/1)
- [COMPLETE LIST OF HTML META TAGS](http://code.lancepollard.com/complete-list-of-html-meta-tags/)
- [微博元标记 Weibo Meta Tags](http://open.weibo.com/wiki/Weibo_meta_tag)

[标签书写的顺序](https://github.com/h5bp/html5-boilerplate/blob/master/dist/doc/html.md#the-order-of-the-title-and-meta-tags)

### 关于 HTML 语义化知道哪些？

[HTML5 Doctor](http://html5doctor.com/)

### 是否有关注 HTML 标准的演进？比较关注哪些方面？能否举一些例子？

- [W3C HTML5 标准](http://www.w3.org/html/)
- [WHATWG HTML 动态标准](https://whatwg.org/)
- [public-html@w3.org mailing list](https://lists.w3.org/Archives/Public/public-html/w)


## CSS

### CSS 有几种引入方式？各自的优缺点？

1. 内嵌 `<style> div { /*...*/ }</style>`

    优点：方便直观
    缺点：只能用于单个页面不利于扩展；没有做到样式与内容分离

2. 外部引入 `<link rel="stylesheet" href="..."/>`

    优点：样式较多的时候易于维护；可复用
    缺点：浏览器缓存，通过在构建阶段给文件名加 hash 解决

3. `@import url(...)`

    优点：比较易于建立起样式文件之间的逻辑联系，易于阅读
    缺点：串行加载，影响网页加载速度。建议在 less/SCSS 源码中使用 import 但是在构建阶段输出成单个文件

4. 内联样式 `<span style="color: red"></span>`

    优点：优先级最高，确保能生效；不用写选择器
    缺点：不易维护；不易扩展

### 不同浏览器上的默认样式，如何处理？（normalize/sanitize）

1. [reset.css](http://meyerweb.com/eric/tools/css/reset/) 去除所有默认样式
2. [normalize.css](https://necolas.github.io/normalize.css/) 尽量使用浏览器默认样式，对于有差异的部分进行统一
3. [sanitize.css](https://10up.github.io/sanitize.css/) 宣称是「更符合程序员直觉」的样式重置

### 盒模型、IE 6/7 与现代浏览器的区别、如何兼容

### BFC 的概念

### containing block 和 stacking context 的概念和计算

### position 和 display 各有几种取值？说说他们的含义与用途

### `position: absolute` 和 `float` 有什么区别

两者都会脱离 normal flow（注意不要翻译成文档流），前者会覆盖 normal flow 中的元素，后者仍然占据位置

### 如何清除浮动？为什么要清除浮动？

### 选择器相关问题
#### specificity 的计算
#### 伪类和伪元素的区分
#### 选择器性能（浏览器如何进行匹配）
#### CSS3 和 CSS4 选择器知道哪些

### CSS 优化

#### 网络加载方面有哪些手段

#### 渲染性能的方面呢

[Reflow & Repaint](http://www.sitepoint.com/10-ways-minimize-reflows-improve-performance/)

### 用过哪些 CSS 方面的工具

### 随便谈谈 CSS 工程化

[CSS STILL SUCKS 2015](http://huangxuan.me/css-sucks-2015/#/)


## JavaScript

### JavaScript 有哪些基本类型

根据 ES2015 标准，JavaScript 的基本类型一共有 7 种，分别是 Undefined、Null、Boolean、String、Symbol、Number 以及 Object，其中 Symbol 是 ES2015 标准中新增的基本类型。

### 区分不同类型的方法有哪些，各有什么问题

### 闭包的概念 & 用途

[Javascript Closures](http://www.jibbering.com/faq/notes/closures/)

### `apply` 和 `call` 的用途和区别

### 原型继承的概念， `prototype` 和 `__proto__` 的区别

### JavaScript 如何实现继承？对象的几种创建方式？

### 是否碰到过内存泄露？能否说一下引起内存泄露的常见原因（网上大部分文章都是跟 IE 相关的，其实没什么必要了解，闭包方面有必要知道）？有什么工具可以调试？

### JavaScript 设计模式知道哪些？Proxy 模式怎么用？

[Learning JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)

### ES6 是否有了解

- 基础
    + [ECMAScript 6入门](http://es6.ruanyifeng.com/)
    + [Understanding ECMAScript 6](https://leanpub.com/understandinges6/read)
- 深入
    + [Exploring ES6](http://exploringjs.com/)

### JavaScript 模块化（常见规范、工具、实现原理）

- 规范 & 工具
    + [JavaScript 模块化七日谈](http://huangxuan.me/2015/07/09/js-module-7day/)
- 实现原理
    + [玩转AMD - 设计思路](http://efe.baidu.com/blog/dissecting-amd-what/)
    + [玩转AMD - 应用实践](http://efe.baidu.com/blog/dissecting-amd-how/)
    + [玩转AMD - Loader](http://efe.baidu.com/blog/dissecting-amd-loader/)
    + [easy.js的模块加载器的详解](http://stylechen.com/easyjs-moduleloader.html)
    + [模块加载器的进化–并行加载](http://stylechen.com/easyjs-parallel-moduleloader.html)
    + [如何实现一个 CMD 模块加载器](http://annn.me/how-to-realize-cmd-loader/)



## DOM

### DOM 的事件机制
#### 冒泡与捕获的概念，如何阻止冒泡
#### Delegation
#### 鼠标点击 a 标签其中会有多少个时间产生
#### 如何区分 dbclick 和 click

### ajax 请求中 readyState 有哪些状态（这个问题我感觉太不常考了……但既然见到过那就收录进来了）

### ajax 跨域

[浅谈WEB跨域的实现（前端向）](http://www.cnblogs.com/vajoy/p/4295825.html)

#### 怎样算是跨域？
#### 跨域的方法有哪些？实现原理是什么？兼容性如何？各自有什么缺点？
#### JSONP 如果页面编码和被请求的资源编码不一致如何处理

### 服务器端消息推送有哪些方法？实现原理？兼容性？缺点？

[关于web通信技术](http://www.tony77.com/archives/431.html)

### jQuery.ready() 实际上是 DOM 中的什么事件？

一般是 `DOMContentLoaded` 事件，不支持时用 `load` 替代

### `window.onload` 和 `$.ready()` 事件有什么区别？

前者是整个网页的所有资源都加载完毕时才触发（包括图片等静态资源），后者在 DOM 树构建完成时就被触发。


## 前端性能优化

### 雅虎 24 条，说出越多越好

### 是否有其他性能优化的经验？


## 页面性能分析

### 页面性能一般可以有哪些指标

- 首字节时间
- 白屏时间
- 首屏时间
- 用户可操作时间
- 总下载时间

### 页面性能记录和分析有哪些方法？除了常见的那些方法之外在现代浏览器里还有其他什么新手段吗？

[7 天打造前端性能监控系统](http://fex.baidu.com/blog/2014/05/build-performance-monitor-in-7-days/)

Navigation Timing API 的支持程度现在已经很广泛了，大部分性能监控系统其实都已经在广泛使用……

### 用过什么性能分析的工具

前一个问题回答的链接里有

## 前端安全

### XSS 的概念、知道哪些解决办法（常规的就行，不必太深入）

[XSS零碎指南](http://www.barretlee.com/blog/2014/05/01/cb-xss-snippets/)

### `escape` / `encodeURI` / `encodeURIComponent` 的区别

### CSRF 攻击的概念、防御手段

### CSP

### 淘宝店铺装修的 CSS 过滤、JS 过滤有什么思路

### 代码质量

主要考察对代码质量检查、单元测试、自动化测试、界面测试、持续集成、持续部署这些理念的概念掌握以及实践


## 后端

### 讲讲 session 的实现原理，cookies 和 session 的关系，客户端禁用 cookies 后怎么使用 session？

### 多台服务器之间该如何共享 session

### 讲讲 RESTful


## NodeJS

### callback hell 以及目前的解决方案

### 用过 koa 吗？thunk 是什么？（等 koa 2 正式版出来以后这个可以不用问了）

### 什么是事件循环？Node 中有哪些类型的函数/调用是异步的？哪些是同步的？

### 怎样绑定 Node 程序到 80 端口[#绑定-node-程序到-80-端口]？

### 有哪些方法可以让 Node 程序遇到错误后自动重启

### 如何实现一个 writable stream？

### Node.js 中怎么删文件？

### 在 Node 中直接用 MySQL 的话，客户端一定时间没有活动的话 MySQL 会断开连接，一般怎么处理这个问题？


## TypeScript

### 都说 TypeScript 的类型系统是 unsound 的，请问这个 unsound 是什么意思？具体表现在什么地方？

### `interface` 和 `declare class` 都可以用来描述一个类，请问这两者的区别是什么？


## 网络

### TCP 三次握手
#### 具体过程
#### 为什么要这么设计

### 说一下网络五层模型（HTTP 协议从应用层到底层都基于哪些协议），HTTP 协议头字段说上来几个，缓存字段是怎么定义的，http 和 https 的区别，在具体使用的时候有什么不一样。是否尽可能详细的掌握 HTTP 协议

### HTTP 状态码
#### 1、2、3、4、5 开头分别表示什么
#### 301 和 302 的区别、为什么要区分
#### 304 表示什么

### 如何防止 304

### `keep-alive`

### cookies 是干嘛的，服务器和浏览器之间的 cookies 是怎么传的，httponly 的 cookies 和可读写的 cookie 有什么区别，有无长度限制，cookies 被禁用后可以考虑用什么替代

### GET/POST 区别

### 一个页面从输入 URL 到页面加载完的过程中都发生了什么事情？越详细越好

### 关于 HTTP2 知道哪些？对未来前端开发可能会有哪些影响？


## 其他

### 会不会用 ps 扣图，png、jpg、gif 这些图片格式解释一下，分别什么时候用。是否了解webp
### 是否了解开源的工具 bower、npm、yeoman、grunt、gulp、webpack，有无用过，有无写过，一个 npm 的包里的 package.json 具备的必要的字段都有哪些（名称、版本号，依赖）


## 手写代码

### walkTheDOM 函数，从 `<body>` 标签起，遍历所有节点并打印标签名

### addClass

### 实现一个简单的 pub-sub 库

### 实现 `_.flatten()`

### object deep clone

### isPrime

### quick sort

### merge sort

### binary search

### throttle & debounce

### 实现 `Object.create()`（不用完全遵循标准，实现蝴蝶书上的版本就够了）

### `Function.prototype.bind`

### CSS 实现元素的水平垂直居中

### 实现一个圣杯布局

### carousel 组件

### 自动补全组件

### overlay 组件

### popup 组件

### drag & drop 组件，分别用 jQuery、MVVM、React 和 RxJS 实现一遍

### 一小时之内写一个扫雷游戏

来源：<http://rkoutnik.com/articles/How-I-Interview.html>

思路/代码：<http://waitingfortheelevator.com/html-5-minesweeper-in-an-hour/>

## 代码实现思路

### 如果要你实现一个 AMD 加载器，你将如何实现？讲一下思路和需要注意的点，最好有伪代码

### Sizzles （jQuery 的选择器模块）的实现思路


## 算法题

### topK

### 翻转单链表

### 反转二叉树

### 单向列表判断是否有环

### LeetCode

<https://leetcode.com/>

[《LeetCode 题解》](https://www.gitbook.com/book/siddontang/leetcode-solution/details) 这本电子书中有很详尽的 C++ 版本的题解。

### careercup
