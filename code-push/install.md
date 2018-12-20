# ubuntu 16.04 安装code-push-server

## 安装nodejs和npm

```shell
curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
sudo apt-get install -y nodejs
```

## 安装 code-push-server

```shell
npm install code-push-server -g
code-push-server-db init --dbhost localhost --dbuser root --dbpassword #初始化mysql数据库
code-push-server #启动服务 浏览器中打开 http://127.0.0.1:3000
```

## 客户端

使用命令安装CodePush终端

```shell
npm install -g code-push-cli
```