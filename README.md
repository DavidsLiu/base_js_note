javascript 高级程序设计读书笔记
========

***只是读书的一些感悟，没有按照书的章节顺序阅读，也算是读到哪里记到哪里吧!***

  什么是JavaScript
  -------
  ***JavaScript由核心（ECMAScript）、DOM(文档对象模型)、BOM（浏览器对象模型）构成***

  文档对象模型（DOM）：不是只针对JavaScript，不过在web浏览器中，基于ECMAScript实现的DOM的确已经成为JavaScript这门语言的一个重要组成部分。
  -----
  DOM1级：DOM Core和DOM HTML。
  
  DOM2级：扩展了DOM Views、 DOM Events、 DOM Style、 DOM Traversal and Range(遍历和操作文档树的接口)
  
  DOM3级：进一步扩展了DOM Load and Save 、DOM Validation,开始支持XML1.0规范
  
  其它DOM: 都是基于XML的，例如：SVG、MathML、SMIL
  
  浏览器对象模型（BOM）：支持访问和操作浏览器窗口
  -----
  扩展包括
    弹出新浏览器窗口
    移动、缩放和关闭浏览器窗口
    浏览器信息navigator
    浏览器加载页面信息location
    用户显示器分辨率信息screen
    对cookie的支持
    XMLHttpRequest和IE的ActiveObject
    
  
  HTML中的JavaScript
  ---------
  <script>元素：在HTML中插入JavaScript就需要<script>元素;
  ***它包含6个属性：async、charset、defer、language、src、type 
  注意：已经设置了src的script不能再其内部插入JavaScript脚本，否则会被忽略，script加载的外部其他域脚本，需要确定其安全性 ***
  
  defer只适用于外部脚本: 脚本放置在head中会影响body内元素的加载，所以尽量放在body内的结束标签前。关于defer属性的使用，它
  是让脚本立即加载，但是得延时到html元素解析完再执行。
  
  async只适用于外部脚本: 
  
  XHTML：可扩展超文本标记语言，在xhtml中植入JavaScript需要加载//<![CDATA[ function(){} //]]> ,所以更加需要通过script在外部植入脚本
  
  
  
  
