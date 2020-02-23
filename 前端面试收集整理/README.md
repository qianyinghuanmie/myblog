
### 参考
 #### 博客
- 1、[中高级前端面试题（万字长文）](https://juejin.im/post/5e4c0b856fb9a07ccb7e8eca)
- 2、[大前端吊打面试官系列](https://juejin.im/post/5e4943d0f265da57537eaba9)
 #### 资料
- 1、[HTML 5 教程](https://www.w3school.com.cn/html5/index.asp)


### 写在前面的话

  因为一些特殊原因在家待了很久，博客和github都很久没有更新了。
  这段时间，代码写的比较少，但是看了不少书。
  因为博主不是科班出身
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

#### 三、js部分

#### 四、浏览器部分


#### 五、常用的一些算法