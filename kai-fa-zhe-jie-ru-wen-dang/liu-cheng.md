### 接入流程

HotApp微信小程序接入只需要在小程序中加入一段代码 var hotapp = require\('utils/hotapp.js'\); 在接入之前需要做一些准备工作。

* 1.注册HotApp小程
 
  序统计账号
* 
* 2.下载js,接入统计
* 
* 3.增加request合法
 
  域名
* 
* 4.接入完成

一行代码接入统计：

```
//app.js
var hotapp = require('utils/hotapp.js');

```

接入示例：

```
//app.js
//HotApp微信小程计接入只需要在小程序的入口文件app.js中引入一行代码:
var hotapp = require('utils/hotapp.js');
//hotapp.setDebug(true); // 显示调试信息开关
App({
  onLaunch: function() { 
    // Do something initial when launch.
  },
  onShow: function() {
      // Do something when show.
  },
  onHide: function() {
      // Do something when hide.
  },
  onError: function(msg) {
    console.log(msg)
  },
  globalData: 'I am global data'
})

```

[sdk 下载](http://wenda.hotapp.cn/article/1)

  


