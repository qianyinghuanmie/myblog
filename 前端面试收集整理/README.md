
### 参考

博客
- 1、[中高级前端面试题（万字长文）](https://juejin.im/post/5e4c0b856fb9a07ccb7e8eca)
- 2、[大前端吊打面试官系列](https://juejin.im/post/5e4943d0f265da57537eaba9)
  
资料
- 1、[HTML 5 教程](https://www.w3school.com.cn/html5/index.asp)
- 2、[CSS3 教程](https://www.w3school.com.cn/css3/index.asp)
- 3、[JavaScript 教程](https://www.w3school.com.cn/js/index.asp)

收费小册
    [前端面试之道](https://juejin.im/book/5bdc715fe51d454e755f75ef/section/5c024ecbf265da616a476638)
    注：某大佬这本收费小册干货很多，有些参考其中的问题，就不列答案了。
### 写在前面的话

  因为一些特殊原因在家待了很久，博客和github都很久没有更新了。
  这段时间，代码写的比较少，但是看了不少书。
  因为博主不是科班出身，在家的几个月把科班的一些书籍都学习了一遍，比如《数据结构》，《计算机组成》，《计算机网络》，《操作系统》，下次有机会，可以把看一些书籍和前端的一些结合来讲，
  现在主要是待业在家，准备出去找工作，因为疫情原因，先对当前的知识做个整理。
  这些整理，只针对于自身的一些问题。
  也有自己觉得一些重要，以及一些感悟的地方。
  
  **ps：前端工作快四年了，准备从上海换回杭州上班，有大佬要人的话，找我呀。哈哈**
### 针对自己的查漏补缺

#### 一、html部分

常见行内元素标签：<code>a、br、code、em、img、input...</code>
常见块级元素标签：<code>div、p、dl、dt、form、h1~h6...</code>

**新特性**
- 用于绘画的 canvas 元素
- 用于媒介回放的 video 和 audio 元素
- 对本地离线存储的更好的支持
- 新的特殊内容元素，比如 article、footer、header、nav、section
- 新的表单控件，比如 calendar、date、time、email、url、search

**知识欠缺点**
 - HTML 5 拖放
 - HTML 5 Canvas
 - TML5 内联 SVG
 - HTML 5 应用程序缓存
 - HTML 5 Web Workers
- HTML 5 服务器发送事件
  
**自己认为重要的一些部分**

- HTML5 Input 类型
- HTML5 表单元素
- HTML5 表单属性

1、HTML5 表单属性，这个感觉很重要

*新的 form 属性：*

    - autocomplete
    - novalidate
  
*新的 form 属性：*

    - autocomplete
    - autofocus
    - form
    - form overrides (formaction, formenctype, formmethod, formnovalidate, formtarget)
    - height 和 width
    - list
    - min, max 和 step
    - multiple
    - pattern (regexp)
    - placeholder
    - required
  
**HTML 事件属性**（重要）
想了想，这部分还单独列出来好了，因为在日常开发中，使用到的概率也比较高

| 属性 | 值 | 描述 |
| :-----| :----: | :---- |
| onafterprint | script | 文档打印之后运行的脚本。 |
| onbeforeprint | script | 文档打印之前运行的脚本。 |
| onbeforeunload | script | 文档卸载之前运行的脚本。 |
| onerror | script | 在错误发生时运行的脚本。 |
| onload(很常用) | script | 页面结束加载之后触发。 |
| onmessage | script | 在消息被触发时运行的脚本 |
| onpagehide(很常用)  | script | 当窗口隐藏时运行的脚本。 |
| onpageshow(很常用)  | script | 当窗口成为可见时运行的脚本。 |
| onresize | script | 当浏览器窗口被调整大小时触发。 |
| onstorage | script | 在 Web Storage 区域更新后运行的脚本。 |
| onunload | script | 一旦页面已下载时触发（或者浏览器窗口已被关闭）。 |

**Form 事件**（重要）

| 属性 | 值 | 描述 |
| :-----| :----: | :---- |
| onblur (很常用) | script | 元素失去焦点时运行的脚本。 |
| onchange(很常用)  | script | 在元素值被改变时运行的脚本。 |
| oncontextmenu | script | 	当上下文菜单被触发时运行的脚本。 |
| onfocus(很常用)  | script | 当元素获得焦点时运行的脚本。 |
| onformchange | script | 在表单改变时运行的脚本。 |
| onforminput | script | 当表单获得用户输入时运行的脚本 |
| oninput(很常用)  | script | 当元素获得用户输入时运行的脚本。 |
| oninvalid(很常用)  | script | 当元素无效时运行的脚本 |
| onselect | script | 在元素中文本被选中后触发。 |
| onsubmit(很常用)  | script | 在提交表单时触发。 |

此外还有

- Keyboard 事件
- Mouse 事件（这块也用的比较多，篇幅原因就不展开列举了，可以自行查看些html5的教程）
- Media 事件

**还有一个比较重要的部分就是video/audio的事件的属性使用了**
[HTML 5 视频/音频参考手册](https://www.w3school.com.cn/tags/html_ref_audio_video_dom.asp)。
使用原生写的时候，做类似的h5活动页，就很有必要参考这块了。

##### *小结：*
    随着几大框架的使用，html5中很多属性的直接应用会变的越来越少，被各种封装，之前公司做的活动页
    也大都是用vue或者react框架下去制作，然后挂在一个路由下面。
    可能在传统公司的使用还是很多，像一些互联网公司面试，问这方面的面试题都很少了。
    撑死了就随便问些新特性啊，行块元素啊，媒体，缓存之类的。

#### 二、css部分

1、盒模型（这个面试10次会问到8次）

 box-sizing: content-box(默认)----指的是标准模型（本身内容宽高度+边框和内边距）

 box-sizing: border-sizing-----指的是IE模型（本身内容的宽高度）

2、flex布局（记得有次面试平安的时候，问的很细，也比较重要）

具体参考[Flex布局教程：语法篇](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)

3、css选择器
因为比较基础，好像问的比较少了，最早的时候还是会问些后代选择器和子选择器之类的。

4、display的值（这个经常问！！！）

5、清浮动（*）

6、posiiton的值：（和display一样，也经常问，这样基础的应该都要掌握）

7、CSS3新特性
- 过渡
- 动画
- 形状转换
- 选择器
- 阴影
- 文字阴影: text-shadow: 2px 2px 2px #000;(水平阴影，垂直阴影，模糊距离，阴影颜色)
- 盒子阴影: box-shadow: 10px 10px 5px #999
- 边框
- 背景
- 文字
- 渐变
- 弹性布局、栅格布局、多列布局
- 媒体查询

8、Sass、Less、Stylus区别
感觉这个问题的即使回答不完全，好像也不是很重要，只要用过其中一种预处理预言，面试官都觉不会在这个问题上纠结太久

9、字体
之所以单独列出来，是因为我们很多图标都开始采用字体的形式，例如阿里字体。

注：**自身欠缺的知识点**
- **动画**（太多的业务代码，导致对动画效果的要求不断的降低）
- **阴影**
- **渐变**
- **背景**（背景用的好的话，真的会有妙用，可惜自身掌握的也不太好。）

 ##### *小结：*

    css一直都重要，特别是布局排版，还有一些兼容部分。
    不管哪次面试，css都是必不可少的环节
    熟练掌握基本的css，在日常的开发会少很多坑
    比如还有什么1像素的问题之类的，都是要在不断的采坑中，慢慢成长的。
    随着css3特性的不断强大，能够代替js做不少动画，好好使用，也会有不错的效果。
    面试之前，应该也要好好把整个css部分，再过一遍


#### 三、js部分

1、js基本数据类型（面试问的概率超高，应该算是基础吧）

undefined、number、string、null、boolean+object ES6新增Symbol

2、var、let、const 三者的区别什么？

    var 存在变量提升，而 let、const 则不会。
    var 的全局声明的变量会挂载到 window 上，而其他两者不会。
    let 和 const 的作用基本一致，后者声明的变量不能再次赋值
注：**有面试官会问你const的声明对象常量，能不能更改对象中的值，建议自己去实现下。。。**

2、原生ajax（以前问的很多，现在框架增多，很多都是请求库，这个反而问的不怎么多了）

    如何创建Ajax
    XMLHttpRequest对象的工作流程
    ==========兼容性写法===========
    var xmlHttp = null;
    if(window.XMLHttpRequset) {
        // IE7+,Firefox,Chrome,Safari,Opera
        xmlHttp = new XMLHttpRequset();
    }
    else {
        // IE5,IE6
        xmlHttp = new ActiveXObject("Microsoft.XMLHTTP")
    }
    兼容性处理
    事件的触发条件
    xmlHttp.onreadystatechange = function() {
        if(xmlHttp.readyState == 4 && xmlHttp.status == 200) {
            responseText、responseXML
        }
    }
    事件的触发顺序
    ======================注意=================
    如果是POST请求则需要添加头
    xmlHttp.setRequestHeader("Content-type": "application/x-www-form-urlencoded")

3、深拷贝，浅拷贝（很常见）

4、Promise的理解和实现（**如果现场要求手写一个promise比较难，我也只能说说思路，这点也比较欠缺诶**）

5、绕不开的闭包问题（问的概率一半一半）

6、原型链

7、map, filter, reduce的作用和区别

8、微任务和宏任务（有次面试网易的时候，有问到，这块要掌握好了，对Event Loop的了解会有很大的收获）

##### *小结：*
    js这部分向来都是问的最多的这块，随着es6的普及，很多次面试都会问es6的东西了。当然es5本身也是
    需要掌握的更加扎实。
    而且后续的使用vue，react等框架，也离不开js的支撑，所以js是务必最需要重视的一块
    


### **总结**

    对html部分和css的部分掌握的还算良好，js却很长时间，因为业务代码的关系，后期一直没有得到良好
    的发展，也没有形成自己的知识体系。
    因为篇幅有限，这期就先写这么多，后续的话，应该是更新
    工程化，HTTP，vue，react，几个框架，
    再往后，也有可能对小程序呀，app之类的，对自身的情况做个总结。