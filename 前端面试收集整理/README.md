
### 参考

**博客**
- 1、[中高级前端面试题（万字长文）](https://juejin.im/post/5e4c0b856fb9a07ccb7e8eca)
- 2、[大前端吊打面试官系列](https://juejin.im/post/5e4943d0f265da57537eaba9)
- 3、[一文速览Webpack](https://juejin.im/post/5d176df351882503221693dc)
- 4、[入门Webpack，看这篇就够了](https://www.jianshu.com/p/42e11515c10f) 注：当初入门的时候看的，可能年代有点的久了，不过这个博主写的真的很不错）
- 5、[三十分钟掌握Webpack性能优化](https://segmentfault.com/a/1190000015883378)
**资料**
- 1、[HTML 5 教程](https://www.w3school.com.cn/html5/index.asp)
- 2、[CSS3 教程](https://www.w3school.com.cn/css3/index.asp)
- 3、[JavaScript 教程](https://www.w3school.com.cn/js/index.asp)
- 4、[webpack 中文文档(v4.15.1)](http://webpack.html.cn/)

**收费小册**
    [前端面试之道](https://juejin.im/book/5bdc715fe51d454e755f75ef/section/5c024ecbf265da616a476638)
    注：某大佬这本收费小册干货很多，有些参考其中的问题，就不列答案了。

github
    [收集的前端面试题和答案]https://github.com/qiu-deqing/FE-interview

### 写在前面的话

  因为一些特殊原因在家待了很久，博客和github都很久没有更新了。
  这段时间，代码写的比较少，但是看了不少书。
  因为博主不是科班出身，在家的几个月把科班的一些书籍都学习了一遍，比如《数据结构》，《计算机组成》，《计算机网络》，《操作系统》，下次有机会，可以把看一些书籍和前端的一些结合来讲，
  现在主要是待业在家，准备出去找工作，因为疫情原因，先对当前的知识做个整理。
  这些整理，只针对于自身的一些问题。
  也有自己觉得一些重要，以及一些感悟的地方。
  
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

#### 四、浏览器部分

1、事件代理
2、跨域
- JSONP
- CORS
- document.domain
- postMessage

3、缓存（cookie，localStorage，sessionStorage，indexDB）

4、Service Worker（这块知识点不太熟）
        Service Worker 是运行在浏览器背后的独立线程，一般可以用来实现缓存功能。使用 Service Worker的话，传输协议必须为 HTTPS。
        因为 Service Worker 中涉及到请求拦截，所以必须使用 HTTPS 协议来保障安全。
    
5、缓存优先级

   - Service Worker
   - Memory Cache
   - Disk Cache
   - Push Cache
   - 网络请求
  
6、浏览器渲染

不得不提到 [从浏览器地址栏输入 url 到显示页面的步骤(以 HTTP 为例)](https://github.com/qiu-deqing/FE-interview)

### 从浏览器地址栏输入 url 到显示页面的步骤(以 HTTP 为例)(这个面试也经常会遇到，自从把《计算机网络》这本书看过了以后，印象深刻了不少)

1. 在浏览器地址栏输入 URL
2. 浏览器查看**缓存**，如果请求资源在缓存中并且新鲜，跳转到转码步骤
   1. 如果资源未缓存，发起新请求
   2. 如果已缓存，检验是否足够新鲜，足够新鲜直接提供给客户端，否则与服务器进行验证。
   3. 检验新鲜通常有两个 HTTP 头进行控制`Expires`和`Cache-Control`：
      - HTTP1.0 提供 Expires，值为一个绝对时间表示缓存新鲜日期
      - HTTP1.1 增加了 Cache-Control: max-age=,值为以秒为单位的最大新鲜时间
3. 浏览器**解析 URL**获取协议，主机，端口，path
4. 浏览器**组装一个 HTTP（GET）请求报文**
5. 浏览器**获取主机 ip 地址**，过程如下：
   1. 浏览器缓存
   2. 本机缓存
   3. hosts 文件
   4. 路由器缓存
   5. ISP DNS 缓存
   6. DNS 递归查询（可能存在负载均衡导致每次 IP 不一样）
6. **打开一个 socket 与目标 IP 地址，端口建立 TCP 链接**，三次握手如下：
   1. 客户端发送一个 TCP 的**SYN=1，Seq=X**的包到服务器端口
   2. 服务器发回**SYN=1， ACK=X+1， Seq=Y**的响应包
   3. 客户端发送**ACK=Y+1， Seq=Z**
7. TCP 链接建立后**发送 HTTP 请求**
8. 服务器接受请求并解析，将请求转发到服务程序，如虚拟主机使用 HTTP Host 头部判断请求的服务程序
9. 服务器检查**HTTP 请求头是否包含缓存验证信息**如果验证缓存新鲜，返回**304**等对应状态码
10. 处理程序读取完整请求并准备 HTTP 响应，可能需要查询数据库等操作
11. 服务器将**响应报文通过 TCP 连接发送回浏览器**
12. 浏览器接收 HTTP 响应，然后根据情况选择**关闭 TCP 连接或者保留重用，关闭 TCP 连接的四次握手如下**：
    1. 主动方发送**Fin=1， Ack=Z， Seq= X**报文
    2. 被动方发送**ACK=X+1， Seq=Z**报文
    3. 被动方发送**Fin=1， ACK=X， Seq=Y**报文
    4. 主动方发送**ACK=Y， Seq=X**报文
13. 浏览器检查响应状态吗：是否为 1XX，3XX， 4XX， 5XX，这些情况处理与 2XX 不同
14. 如果资源可缓存，**进行缓存**
15. 对响应进行**解码**（例如 gzip 压缩）
16. 根据资源类型决定如何处理（假设资源为 HTML 文档）
17. **解析 HTML 文档，构件 DOM 树，下载资源，构造 CSSOM 树，执行 js 脚本**，这些操作没有严格的先后顺序，以下分别解释
18. **构建 DOM 树**：
    1. **Tokenizing**：根据 HTML 规范将字符流解析为标记
    2. **Lexing**：词法分析将标记转换为对象并定义属性和规则
    3. **DOM construction**：根据 HTML 标记关系将对象组成 DOM 树
19. 解析过程中遇到图片、样式表、js 文件，**启动下载**
20. 构建**CSSOM 树**：
    1. **Tokenizing**：字符流转换为标记流
    2. **Node**：根据标记创建节点
    3. **CSSOM**：节点创建 CSSOM 树
21. **[根据 DOM 树和 CSSOM 树构建渲染树](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-tree-construction)**:
    1. 从 DOM 树的根节点遍历所有**可见节点**，不可见节点包括：1）`script`,`meta`这样本身不可见的标签。2)被 css 隐藏的节点，如`display: none`
    2. 对每一个可见节点，找到恰当的 CSSOM 规则并应用
    3. 发布可视节点的内容和计算样式
22. **js 解析如下**：
    1. 浏览器创建 Document 对象并解析 HTML，将解析到的元素和文本节点添加到文档中，此时**document.readystate 为 loading**
    2. HTML 解析器遇到**没有 async 和 defer 的 script 时**，将他们添加到文档中，然后执行行内或外部脚本。这些脚本会同步执行，并且在脚本下载和执行时解析器会暂停。这样就可以用 document.write()把文本插入到输入流中。**同步脚本经常简单定义函数和注册事件处理程序，他们可以遍历和操作 script 和他们之前的文档内容**
    3. 当解析器遇到设置了**async**属性的 script 时，开始下载脚本并继续解析文档。脚本会在它**下载完成后尽快执行**，但是**解析器不会停下来等它下载**。异步脚本**禁止使用 document.write()**，它们可以访问自己 script 和之前的文档元素
    4. 当文档完成解析，document.readState 变成 interactive
    5. 所有**defer**脚本会**按照在文档出现的顺序执行**，延迟脚本**能访问完整文档树**，禁止使用 document.write()
    6. 浏览器**在 Document 对象上触发 DOMContentLoaded 事件**
    7. 此时文档完全解析完成，浏览器可能还在等待如图片等内容加载，等这些**内容完成载入并且所有异步脚本完成载入和执行**，document.readState 变为 complete,window 触发 load 事件
23. **显示页面**（HTML 解析过程中会逐步显示页面）

7、重绘（Repaint）和回流（Reflow）（经典的前端问题，经常会遇见）

### 5、安全问题

1、xss攻击（[百度百科](https://baike.baidu.com/item/XSS%E6%94%BB%E5%87%BB/954065?fr=aladdin)）
一般的解决方案就是转义输入输出的内容，对于引号、尖括号、斜杠进行转义。

2、CSRF（[百度百科](https://baike.baidu.com/item/%E8%B7%A8%E7%AB%99%E8%AF%B7%E6%B1%82%E4%BC%AA%E9%80%A0/13777878?fromtitle=CSRF&fromid=2735433&fr=aladdin)）
防范 CSRF 攻击可以遵循以下几种规则：
- Get 请求不对数据进行修改
- 不让第三方网站访问到用户 Cookie
- 阻止第三方网站请求接口
- 请求时附带验证信息，比如验证码或者 Token
  
3、点击劫持

###6、性能问题
1、图片优化

2、节流

3、防抖

4、预加载

5、预渲染

6、懒加载

7、懒执行

8、cdn

### 7、webpack

*图片来源于http://webpack.html.cn/*
![img](http://webpack.html.cn/img/webpack.png)

核心概念
- 入口
- 输出
- 模块
- 加载器
- 插件
- 配置

1、webpack的构建过程

    1.1. 初始化参数，从配置文件和shell语句中读到的参数合并，得到最后的参数
    1.2. 开始编译：用合并得到的参数初始化complier对象，加载是所有配置的插件，执行run方法开始编译
    1.3. 确定入口，通过entry找到入口文件
    1.4. 编译模块，从入口文件出发，调用所有配置的loader对模块进行解析翻译，在找到该模块依赖的模块进行处理
    1.5. 完成模块编译，得到每个模块被翻译之后的最终的内容和依赖关系
    1.6. 输出资源，根据入口和模块之间的依赖关系，组装成一个个包含多个模块的chunk，在把每个chunk转换成一个单独的文件加载到输出列表
    1.7. 输出完成，确定输出的路径和文件名，把内容写到文件系统中
    在以上过程中，webpack会在特定的时间点广播出特定的事件，插件在舰艇感兴趣的事件后会执行特定的逻辑，改变webpack的运行结果


2、loader 和 plugin 有什么区别

       loader 用于对模块的源代码进行转换。loader 可以使你在 import 或"加载"模块时预处理文件。因
    此，loader 类似于其他构建工具中“任务(task)”，并提供了处理前端构建步骤的强大方法。loader 可
    以将文件从不同的语言（如 TypeScript）转换为 JavaScript，或将内联图像转换为 data URL。
    loader 甚至允许你直接在 JavaScript 模块中 import CSS文件！ 因为 webpack 本身只能处理 
    JavaScript，如果要处理其他类型的文件，就需要使用 loader 进行转换，loader 本身就是一个函数，
    接受源文件为参数，返回转换的结果。
       Plugin 是用来扩展 Webpack 功能的，通过在构建流程里注入钩子实现，它给 Webpack 带来了很大
    的灵活性。 通过plugin（插件）webpack可以实 loader 所不能完成的复杂功能，使用 plugin 丰
    富的自定义 API 以及生命周期事件，可以控制 webpack 打包流程的每个环节，实现对 webpack 的
    自定义功能扩展。

3、怎么区分开发环境和正式环境

            if(process.env.NODE_ENV === "production") {
                console.log("你正在线上环境")
            }else {
            console.log("你正在使用开发环境")
            }  

4、webpack如何优化性能