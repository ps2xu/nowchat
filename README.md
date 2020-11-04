# 搭建DuckChat（鸭信） – 一款简单好用的聊天系统

2020年2月26日*11:14:06*[ 7](https://www.daniao.org/8303.html#comments) 8,519 940字阅读3分8秒



DuckChat 是一套完整的私有即时通讯（instant message）解决方案，含服务器端程序、客户端（含iOS、Android、PC等）程序。通过DuckChat，站点管理员可以快速的在自己服务器上搭建起一套私有的即时通讯服务，用户可以使用客户端连接至此服务器进行信息交互。

但是不知道怎么没人维护了，官网也没了，安装文档一个找不到。不过还能再github上看到项目，而且最近的更新是在一年前，还好，不算太久远，搭建好了还是可以正常使用的。今天这篇文章就来说说如何用宝塔面板搭建DuckChat（鸭信）！！！类似的文章如下：



[宝塔面板安装fiora – 一款有趣的多人在线网络聊天系统](https://www.daniao.org/8056.html)



## 具体的安装和部署

------



#### 1、前言

github：https://github.com/duckchat/gaga

下载：https://github.com/duckchat/gaga/releases



#### 2、准备

- 宝塔面板
- PHP版本>=7(不支持7.3)
- nginx
- mysql5.x
- 域名解析好
- 新建网站
- 新建好数据库



#### 3、部署

**1》下载**

新建好网站，进入网站根目录，用远程下载把程序下载到本地，如图：

[![宝塔面板搭建DuckChat（鸭信） – 一款简单好用的聊天系统](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-1.png)](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-1.png)

**注意**：下载好之后把“**src**”里的文件复制到网站根目录即可。

**2》安装**

浏览器输入你的准备好的域名，就开始了安装，同意协议之后，会检测站点信息，如图：

[![宝塔面板搭建DuckChat（鸭信） – 一款简单好用的聊天系统](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-2.png)](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-2.png)

点击下一步，就需要你填写数据库信息了，这我们可以选择自带的轻量级的数据库“sqlite”，或者用mysql数据库。如图：

[![宝塔面板搭建DuckChat（鸭信） – 一款简单好用的聊天系统](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-3.png)](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-3.png)

点击“初始化站点”即可安装成功，会出现登录的界面，如图：

[![宝塔面板搭建DuckChat（鸭信） – 一款简单好用的聊天系统](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-4.png)](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-4.png)



#### 4、简单使用

登录之后，可以创建群聊。如图：

[![宝塔面板搭建DuckChat（鸭信） – 一款简单好用的聊天系统](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-5.png)](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-5.png)

群聊就和微信差不多了，可以发图片，资源，聊天等，如图：

[![宝塔面板搭建DuckChat（鸭信） – 一款简单好用的聊天系统](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-6-min.png)](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-6-min.png)

发出的消息、图片、资源等，和微信一样也是可以撤回的。



#### 5、一些问题

PHP版本>=7(不支持7.3)，不然安装会出问题。

如果不能发图片，需要把网站目录权限修改为777

支持ssl，可以在宝塔面板申请ssl证书，强制301后就会自动开启。

支持Android、iOS的app，这个没测试过。

[![宝塔面板搭建DuckChat（鸭信） – 一款简单好用的聊天系统](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-7.png)](https://www.daniao.org/wp-content/uploads/2020/02/duckchat-bt-dn-7.png)



#### 6、最后

因为这个项目已经没人维护了，最近的版本也是2018年11月份的版本，所以，如果出了问题，都要靠自己解决了。

但是使用体验还算不错，一个免费的项目，能做到这样也不错了。可惜的是，现在官网都么了。
