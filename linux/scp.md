# linux scp

## 上传到远端

+ 上传目录

```shell
scp -r ./util 用户名@192.168.1.65:/home/wwwroot/limesurvey_back/scp
```

+ 上传文件

```shell
scp ./util 用户名@192.168.1.65:/home/wwwroot/limesurvey_back/scp
```

如果制定了用户名，后面只要输入密码就行了，如果没有写用户名 就要输入用户名 和密码

## 远端下载

```shell
scp  -r   jiangzhaowei@211.154.xxx.xxx:/kk/jiangzhaowei/share/webCompileOut.sql     ./
```

注意：

如果是目录拷贝要加“-r”参数，用户名可选，如果省略用户名，默认为终端的用户名。