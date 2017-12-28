### **1. 关于APP ID 和 Secret：**

打开芝麻统计首页，可以看到APP ID 和 Secret ,相应的APP ID 和 Secret 可以登录**微信公众平台小程序开发的“设置”**界面查看：

注意：不可直接使用服务号或订阅号的 AppID 



[![](/assets/QQ截图20171228174725.png "20170124-1lqy")](https://blogcdnimg.clewm.net/2017/01/20170124-1lqy.png)

[![](/assets/QQ截图20171228174848.png "20170124-2lqy")](https://blogcdnimg.clewm.net/2017/01/20170124-2lqy.png)

### **2. 参数路径如何填写**

参数路径基于小程序代码进行设置。

比如：小程序的参数路径，二维码扫描打开后需要进入text界面，而不是默认界面，我们即可设置参数为：

pages/text/text?query=1

然后生成的二维码扫描后就会直接今天text界面，而在text界面也能获取到参数为query的值。

[](https://blogcdnimg.clewm.net/2017/01/20170124-3lqy.png)

