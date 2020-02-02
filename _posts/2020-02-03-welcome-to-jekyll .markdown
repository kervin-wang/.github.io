---
layout: Service
title:  "Vultr 搭建服务器"
date:   2020-02-03 20:00:36 +0530
categories: vultr service
---
### 服务器搭建

首先登录https://my.vultr.com/，进入账户

进入账户后，选择蓝色的加号，如下图

![image-20200202200201462](https://github.com/kervin-wang/blog.github.io/blob/master/_image/image-20200202200201462.png?raw=true)

点击加号后，会出现服务器的选择项，按照自己的需求选择，

![image-20200202200315023](C:\Users\Administrator\Documents\GitHub\blog.github.io\_image\image-20200202200315023.png)

选择到Additional Features之后，都可以不用勾选，默认配置

![image-20200202200422696](C:\Users\Administrator\Documents\GitHub\blog.github.io\_image\image-20200202200422696.png)

成功后会出现下面的画面

![image-20200202200859994](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200202200859994.png)

在图中黑色涂抹处点击，可以看到服务器的更加详细的信息

![image-20200202200959848](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200202200959848.png)

### shadowsocket安装

服务器搭建以后，需要下载shadowsocket完成个人电脑与服务器的ssh交互，

为了方便操作，可以使用Xshell或者puty或者MobaXterm完成对服务器的操作，

当然vultr也提供了网页操作的界面，在上图右上角电源图标左侧的电脑图标，点击即可进入服务器远程桌面，但是这种方法不可以在服务器上使用个人电脑的复制粘贴功能，还是推荐使用上述的Xshell等

工具

下面以Xshell为例

Xshell登录到服务器，服务器的IP，用户名和密码都可以在上一副中获得

登录进去后，需要进行shadowsocket的安装，

```
wget --no-check-certificate -O shadowsocks.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks.sh

chmod +x shadowsocks.sh

./shadowsocks.sh | tee shadowsocks.log
```

安装过程如下：

![16](C:\Users\Administrator\Desktop\16.png)

![17](C:\Users\Administrator\Desktop\17.png)

![18](C:\Users\Administrator\Desktop\18.png)

等待安装完成

### 连接SS

下载Shadowsockets，并按照上副图中的红色信息配置服务器，并启动代理



至此安装结束，

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
