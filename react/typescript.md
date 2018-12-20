# TypeScript与React结合起来使用

## 安装create-react-app

我们之所以使用create-react-app是因为它能够为React工程设置一些有效的工具和权威的默认参数。 它仅仅是一个用来搭建React工程的命令行工具而已。

```shell
npm install -g create-react-app
```

## 创建新工程

让我们首先创建一个叫做my-app的新工程：

```shell
create-react-app my-app --scripts-version=react-scripts-ts
```

注意：

+ tsconfig.json包含了工程里TypeScript特定的选项。
+ tslint.json保存了要使用的代码检查器的设置，TSLint。
+ package.json包含了依赖，还有一些命令的快捷方式，如测试命令，预览命令和发布应用的命令。
+ public包含了静态资源如HTML页面或图片。除了index.html文件外，其它的文件都可以删除。
+ src包含了TypeScript和CSS源码。index.tsx是强制使用的入口文件。