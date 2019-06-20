# Fiddler + Proxifier 教程

# abstract

小白找了半天终于学会如何使用 Fiddler + Proxifier 抓取任意程序的包, 记录一下:

# 流程简介

+ 1.配置 Fiddler 的监控端口
+ 2.配置 Proxifier 的代理服务器 到 刚刚配置的的Fiddler 的监控端口
+ 3.配置 Proxifier 的代理规则 到 刚刚配置的的Proxifier 的服务器 

# 图片演示:

1. 先下载  Fiddler 和 Proxifier

2.  配置 Fiddler 的监控端口

   2.1 Fiddler -> 工具-> Fiddler 选项->会话->Fiddler监听端口 ->8888

   ![配置 Fiddler 的监控端口](https://i.loli.net/2019/06/12/5d00c72b8160f54131.jpg)

 2.配置 Proxifier 的代理服务器 到 刚刚配置的的Fiddler 的监控端口

 	2.1 Proxifier -> 配置文件 ->  代理服务器 ->设置为本地ip 127.0.0.1 端口值为上面Fiddler 检测的端口

​	![设置为本地ip 127.0.0.1 端口值为上面Fiddler 检测的端口](https://i.loli.net/2019/06/12/5d00c78bb9e8421217.png)



3. 配置 Proxifier 的代理规则 到 刚刚配置的的Proxifier 的服务器 

   3.1 Proxifier 配置文件 代理规则, 把你要监视的exe 填上 并设置刚刚配置的 代理服务器 如图 test

   名称随便填, 应用程序填要检测的程序名字 动作选刚刚新建的 代理服务器(127.0.0.1:8888)

   ![配置 Proxifier 的代理规到刚刚配置的的Proxifier的服务器](https://i.loli.net/2019/06/12/5d00c7f22ab4085629.png)4. 下面是结果图:
   ![结果图](https://i.loli.net/2019/06/12/5d00c84089a0f43590.png)
   写的不是很详细, 有问题问吧...
