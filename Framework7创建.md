Framework7 CLI是一个功能非常强大的工具，也是开始Framework7应用程序开发的推荐方法
1、首先，确保您已经安装了Cordova
npm install -g cordova 
2、安装Framework7 CLI
npm install -g framework7-cli
3、假如安装过程中遇到与访问错误有关的问题，可以尝试运行带有其他标志的命令
npm install -g framework7-cli --unsafe-perm=true --allow-root

一、要建立应用程序
framework7 create
会提示您要开始使用的框架和模板问题

二、创建应用程序用户界面
framework7 create --ui
1、它将启动UI，您可以在其中配置项目。默认情况下，它将在localhost:3001地址上启动服务器。如果要更改端口，请使用--port <n>参数：
framework7 create --ui --port 8080

三、使用自定义图标
在创建的项目中有一个assets-src目录。它包含必需的图标和初始屏幕源图像。要生成自己的图标和启动屏幕图像，
您将需要用自己的图像替换此目录中的所有资产（注意图像的大小和格式），并在项目目录中运行以下命令：
 framework7 generate-assets
就是说，脚本将生成所有所需大小的图标和启动屏幕，并自动将它们放置在需要的位置。

