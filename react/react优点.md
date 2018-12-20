# react优点

## react组件

+ React 组件可以让你把UI分割为独立、可复用的片段，并将每一片段视为相互独立的部分。

## json轻量级

## typescript

+ TypeScript是一门支持ES6规范的语言
+ 在Typescript里面是运行为变量指定类型的，比如当你为这个变量指定数字类型的值的时候，IDE会做出类型检查，然后告诉你这里可能会有错误，这个特性会减少你在开发阶段犯错误的几率。
+ 在IDE里面去编写TypeScript的代码时，IDE会根据你当前的上下文，把你能用的类、变量、方法和关键字都给你提示出来，你只要直接去选就可以了，这个特性会大大提升你的开发效率
+ angular2以后是使用typescript来编写的

## reactnative 优点

+它允许移动APP开发人员以更快的部署时间和更短的开发周期创建性能更好的APP。React Native开发也是一个由数以千计的反应原生开发人员组成的大型团队。开发人员更喜欢使用React Native开发对于APP开发，因为APP不仅可以更快地构建，而且可以立即重新加载，而无需重新编译。当开发人员启用“实时重新加载”选项时，移动APP将自动编译，因此不需要每次运行APP，我们都可以立即获得对UI的反思。这为移动APP开发人员提供了快速开发环境。由于React Native开发允许开发人员同时使用React Native和Native代码，所以优化移动APP的特定方面也更加容易。

### React Native应用是真正的移动应用

React Native产出的并不是“网页应用”， 或者说“HTML5应用”，又或者“混合应用”。 最终产品是一个真正的移动应用，从使用感受上和用Objective-C或Java编写的应用相比几乎是无法区分的。 React Native所使用的基础UI组件和原生应用完全一致。

### 别再傻等编译了！

React Native让你可以快速迭代开发应用。 比起传统原生应用漫长的编译过程，现在你可以在瞬间刷新你的应用。开启Hot Reloading的话，甚至能在保持应用运行状态的情况下热替换新代码！ 试试看吧，包你双击666。

### 可随时呼叫原生外援

React Native完美兼容使用Objective-C、Java或是Swift编写的组件。 如果你需要针对应用的某一部分特别优化，中途换用原生代码编写也很容易。 想要应用的一部分用原生，一部分用React Native也完全没问题 —— Facebook的应用就是这么做的。

## redux

Redux 是 JavaScript 状态容器，提供可预测化的状态管理。 (如果你需要一个 WordPress 框架，请查看 Redux Framework。)

可以让你构建一致化的应用，运行于不同的环境（客户端、服务器、原生应用），并且易于测试。不仅于此，它还提供 超爽的开发体验，比如有一个时间旅行调试器可以编辑后实时预览。

Redux 除了和 React 一起用外，还支持其它界面库。 它体小精悍（只有2kB，包括依赖）。

## 异步

单进程，无阻塞

## websocket

+ 节约带宽。不停地轮询服务端数据这种方式，使用的是http协议，head信息很大，有效数据占比低， 而使用WebSocket方式，头信息很小，有效数据占比高。
+ 无浪费。 轮询方式有可能轮询10次，才碰到服务端数据更新，那么前9次都白轮询了，因为没有拿到变化的数据。 而WebSocket是由服务器主动回发，来的都是新数据。
+ 实时性，考虑到服务器压力，使用轮询方式不可能很短的时间间隔，否则服务器压力太多，所以轮询时间间隔都比较长，好几秒，设置十几秒。 而WebSocket是由服务器主动推送过来，实时性是最高的

### socket.io

+ Socket.IO是一个完全由JavaScript实现、基于Node.js、支持WebSocket的协议用于实时通信、跨平台的开源框架，它包括了客户端的JavaScript和服务器端的Node.js。Socket.IO除了支持WebSocket通讯协议外，还支持许多种轮询（Polling）机制以及其它实时通信方式，并封装成了通用的接口，并且在服务端实现了这些实时机制的相应代码。Socket.IO实现的Polling通信机制包括Adobe Flash Socket、AJAX长轮询、AJAX multipart streaming、持久Iframe、JSONP轮询等。Socket.IO能够根据浏览器对通讯机制的支持情况自动地选择最佳的方式来实现网络实时应用。
+ Socket.IO已经具有众多强大功能的模块和扩展API，如（session.socket.io)（http session中间件，进行session相关操作）、socket.io-cookie（cookie解析中间件）、session-web-sockets（以安全的方式传递Session）、socket-logger（JSON格式的记录日志工具）、websocket.MQ（可靠的消息队列）、socket.io-mongo（使用MongoDB的适配器）、socket.io-redis（Redis的适配器）、socket.io-parser（服务端和客户端通讯的默认协议实现模块）等。
+ Socket.IO实现了实时、双向、基于事件的通讯机制,它解决了实时的通信问题，并统一了服务端与客户端的编程方式。启动了Socket以后，就像建立了一条客户端与服务端的管道，两边可以互通有无。它还能够和Express.js提供的传统请求方式很好的结合，即可以在同一个域名，同一个端口提供两种连接方式：