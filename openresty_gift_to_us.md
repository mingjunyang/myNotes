OpenResty可以给我们的开发带来什么
---
1. Nginx简介
  * [nginx](http://nginx.org/en/docs/)
1. OpenResty和Nginx之间的关系。
  * [lua-resty-core](https://github.com/openresty/lua-resty-core)
  * RPC与FFI之间的比较

1. Nginx的起源和发展。
  * 异步轻松解决了C10K难题。NodeJS也异步高性能IO发家。
  * 比Apache的内存消耗低。
  * 轻量有功能丰富。
  * 模块化设计做的很好。

1. Nginx的常见用法。
  * 静态文件服务
  * http代理、反向代理
  * load balance
  * 邮件代理
  * web cache

1. Nginx扩展模块虽然开发起来还是比较简单，但是前提是得会C，还得非常熟悉Nginx。
  eq. [nginx-upload-module](https://github.com/vkholodkov/nginx-upload-module)
1. Nginx你只能写死一些配置，或者用一些正则，或者用一些简单的规则。

1. 在nginx的基础上做一些事情
  * tengine(增强Nginx的能力，主要服务Ali系的需求，目前以维护和为主)。
    Tengine is a web server originated by Taobao, the largest e-commerce website in Asia. It is based on the Nginx HTTP server and has many advanced features. Tengine has proven to be very stable and efficient on some of the top 100 websites in the world, including taobao.com and tmall.com.
    Tengine has been an open source project since December 2011. It is being actively developed by the Tengine team, whose core members are from Taobao, Sogou and other Internet companies. Tengine is a community effort and everyone is encouraged to get involved.

  * 2015-09-23出现在github上的njs项目(增强配置的灵活性)。
    Configure nginx with HTTP and Stream JavaScript modules。

  * 2010-01-20 first commit的openresty(全功能Web服务器的目标)。
    OpenResty - Turning Nginx into a Full-Fledged Scriptable Web Platform.
    A Fast and Scalable Web Platform by Extending NGINX with Lua.

1. Lua语言与LuaJIT(嵌入式领域，游戏脚本领域，轻量级语言的领域)。[Lua](https://www.lua.org/about.html) is a powerful, efficient, lightweight, embeddable scripting language. It supports procedural programming, object-oriented programming, functional programming, data-driven programming, and data description.
  Lua combines simple procedural syntax with powerful data description constructs based on associative arrays and extensible semantics. Lua is dynamically typed, runs by interpreting bytecode with a register-based virtual machine, and has automatic memory management with incremental garbage collection, making it ideal for configuration, scripting, and rapid prototyping.

  Lua只有一种数据类型，就是Table。有编程语言基础之后，只要再熟悉一下Openresty的API，再有点想法就很容易上手。

1. OpenResty怎么去做这些的。
  * [lua-resty-core](https://github.com/openresty/lua-resty-core)
  * [lua-nginx-module](https://github.com/openresty/lua-nginx-module)
  * [LuaJIT](https://github.com/LuaJIT/LuaJIT)

1. OpenResty的一些使用姿势。
1. 配合Docker我们玩得更嗨。
  * [base_openresty](https://coding.net/t/trustasia/p/incubators/git/tree/master/base_openresty)

1. 资源
  * [OpenResty最佳实践](https://www.gitbook.com/book/moonbingbing/openresty-best-practices/details)
  * [ginx开发从入门到精通](http://tengine.taobao.org/book/index.html)
  * [nginx原理解析篇](http://tengine.taobao.org/book/source_analysis.html)
  * [执行阶段概念](https://moonbingbing.gitbooks.io/openresty-best-practices/content/ngx_lua/phase.html)
