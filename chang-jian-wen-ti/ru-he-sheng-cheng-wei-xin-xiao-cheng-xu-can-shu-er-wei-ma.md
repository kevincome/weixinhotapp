### **1. 关于APP ID 和 Secret：**

打开草料小程序参数二维码生成界面，可以看到APP ID 和 Secret ,相应的APP ID 和 Secret 可以登录**微信公众平台小程序开发的“设置”**界面查看：

[![](https://blogcdnimg.clewm.net/2017/01/20170124-1lqy-1024x409.png "20170124-1lqy")](https://blogcdnimg.clewm.net/2017/01/20170124-1lqy.png)

[![](https://blogcdnimg.clewm.net/2017/01/20170124-2lqy-1024x515.png "20170124-2lqy")](https://blogcdnimg.clewm.net/2017/01/20170124-2lqy.png)

### **2. 关于参数路径**

参数路径基于小程序代码进行设置。

比如：小程序的参数路径，二维码扫描打开后需要进入text界面，而不是默认界面，我们即可设置参数为：

pages/text/text?query=1

然后生成的二维码扫描后就会直接今天text界面，而在text界面也能获取到参数为query的值。

[![](https://blogcdnimg.clewm.net/2017/01/20170124-3lqy.png "20170124-3lqy")](https://blogcdnimg.clewm.net/2017/01/20170124-3lqy.png)

