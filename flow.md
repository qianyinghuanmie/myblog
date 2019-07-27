### 你真的熟练使用webpack吗？

- *https://www.webpackjs.com/* 官网地址

当自己在简历中写着熟练使用webpack的时候，殊不知自己只是在vue脚手架，react脚手架的路上走着比较轻松而已。

###### 当面试官问你这几个问题的时候，你还能从容答上来吗(高手请忽略)

 - 什么是webpack，webpack的打包过程是怎么样的？
 - webpack基础配置的属性有哪些
 - 什么是loader?什么是plugin?他们执行先后关系是什么？
 - 提高webpack的构建速度(这个比较广泛)
 - 是否自己写过plugin(一旦你回答写过，马上问题就来了)
 - 是否用过compiler ，介绍其中几个方法？

### 正文

    先抛开这几个问题。谈谈本人正常学习webpack的过程，由于几年前先接触的vue，一套vue-cli跑下来 ，生成demo以后感觉自己不仅

    学会了vue，还精通了webpack。

    后面有个偶然的机会，想自己从头使用webpack部署。才知道里面没有那么简单。

这里有个参考的文章:
    
[入门Webpack，看这篇就够了](https://www.jianshu.com/p/42e11515c10f)。

感兴趣的可以自己看。

### webpack的打包过程是怎么样的

    这个当自己实践着一步步去尝试开始的时候的，会有个比较清晰的理解的。

    webpack是一个打包模块化javascript的工具，在webpack里一切文件皆模块，

    通过loader转换文件，通过plugin注入钩子，最后输出由多个模块组合成的文件，

    webpack专注构建模块化项目。

### webpack基础配置的属性有哪些

- 入口(entry)
- 输出(output)
- loader
- 插件(plugins)
  
当然在实际工程中，看到的的webpack的配置属性远远没有这么简单。

比如：我们会环境配置。dev,pro等等。

可能会使用到代理配置:类似于下面代码所示，用来进行跨域配置

```
 proxyTable: {
      '/api': {
        target: 'http://……………………',
        changeOrigin: true,
        pathRewrite: {
          '^/api': '/api'
        }
      },
 }
```
  
######
    每个属性的配置都可以延伸开，比如入口，可以是单入口，也可以是多入口。

    一旦用到具体的场景的话。

    每个配置项都有可能变得复杂起来。

###  什么是loader?什么是plugin?他们执行先后关系是什么？

    loader 用于对模块的源代码进行转换。
    
    loader 可以使你在 import 或"加载"模块时预处理文件。
    
    因此，loader 类似于其他构建工具中“任务(task)”，并提供了处理前端构建步骤的强大方法。

######
    插件是 webpack 的支柱功能。
    
    webpack 自身也是构建于，你在 webpack 配置中用到的相同的插件系统之上！

    插件目的在于解决 loader 无法实现的其他事。

**自然而然，这样通过描述，就能比较清晰的理解的。**

**plugin是在loader之后执行的，当loader处理完模块代码，plugin继续处理loader未能做完的事情**


### 提高webpack的构建速度

这里有的一篇文章介绍的比较详细

https://www.jianshu.com/p/bb1e76edc71e

当然优化的点大致可以区分下

    - 选用合适的loader，这个是比较重要的，能够有效的提升webpack编译的速度。
  
    - 使用Happypack 实现多线程加速编译。
  
    - 不需要打包编译的插件库换成全局"script"标签引入的方式
  
    - 开启缓存
  
### 什么是compiler

    这个只有当自己真正去写插件的时候，才会意识到的。

[compiler](https://www.webpackjs.com/api/compiler-hooks/)

######
    Compiler 模块是 webpack 的支柱引擎，它通过 CLI 或 Node API 传递的所有选项，
    
    创建出一个 compilation 实例。它扩展(extend)自 Tapable 类，以便注册和调用插件。
    
    大多数面向用户的插件，会先在 Compiler 上注册。

**以下生命周期钩子函数，**

| 生命周期             |                                          说明                                           |
| :------------------- | :-------------------------------------------------------------------------------------: |
| entryOption          |                           在 entry 配置项处理过之后，执行插件                           |
| afterPlugins         |                              设置完初始插件之后，执行插件                               |
| afterResolvers       |                            resolver 安装完成之后，执行插件。                            |
| environment          |                           environment 准备好之后，执行插件。                            |
| afterEnvironment     |                          environment 安装完成之后，执行插件。                           |
| beforeRun            |                         compiler.run() 执行之前，添加一个钩子。                         |
| run                  |                    开始读取 records 之前，钩入(hook into) compiler。                    |
| watchRun             | 监听模式下，一个新的编译(compilation)触发之后，执行一个插件，但是是在实际编译开始之前。 |
| normalModuleFactory  |                        NormalModuleFactory 创建之后，执行插件。                         |
| contextModuleFactory |                        ContextModuleFactory 创建之后，执行插件。                        |
| beforeCompile        |                        编译(compilation)参数创建之后，执行插件。                        |
| compile              |              一个新的编译(compilation)创建之后，钩入(hook into) compiler。              |
| thisCompilation      |                触发 compilation 事件之前执行（查看下面的 compilation）。                |
| compilation          |                          编译(compilation)创建之后，执行插件。                          |
| make                 |                                           ……                                            |
| afterCompile         |                                           ……                                            |
| shouldEmit           |                                          ……。                                           |
| needAdditionalPass   |                                           ……                                            |
| afterEmit            |                              生成资源到 output 目录之后。                               |
| done                 |                                 编译(compilation)完成。                                 |
| failed               |                                 编译(compilation)失败。                                 |
| invalid              |                                监听模式下，编译无效时。                                 |
| watchClose           |                                     监听模式停止。                                      |

**实际应用的时候，大概只需要上面几个编译前，编译后的几个钩子**

###最后

    请原谅偶只是个标题党，文章也只是大致介绍的webpack所有需要了解的知识点的大概范围。
    
    在实际场景应用的时候，各不相同。

    