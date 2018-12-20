# code-push-cli常用命令

应用名：RNFootPath-android

```shell
code-push login http://xxx.xxx.xxx.xxx:3000
code-push-server
code-push app add RnDemo-android android react-native
```

快速打包：

```shell
code-push release-react RNFootPath-android android
code-push app ls
code-push deployment add  #部署
code-push deployment rename #重命名
code-push deployment rm #删除部署
code-push deployment ls #列出应用的部署情况
code-push deployment ls -k #查看部署的key
code-push deployment history #查看历史版本(Production 或者 Staging)
#测试版本更新：
code-push deployment history 应用名 Staging
#生产版本更新：
code-push deployment history RNFootPath-android Production
#应用创建时有两个环境，一个是Staging，一个是Production,开发阶段用Staging，开发完成可以用code-push promote 将应用迁移到Production中。
#可以对一小部分用户进行升级测试：
code-push promote RNFootPath-android Staging Production -r 20%
#软件稳定后，可以全面发布：
code-push patch RNFootPath-android Production -r 100%
```