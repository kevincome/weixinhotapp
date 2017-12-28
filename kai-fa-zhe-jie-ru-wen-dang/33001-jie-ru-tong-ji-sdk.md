### 接入统计SDK {#document_step_2}

1、下载统计 JS SDK

HotApp小程序统计 js sdk 下载地址[点击下载统计 js sdk](http://wenda.hotapp.cn/article/1)[小程序统计demo 下载](http://wenda.hotapp.cn/article/1)

将js文件放入utils 目录，或其它目录。\(注意：hotapp.js 与 hotapp-conf.js 必须位于同一目录\)

2、修改 hotapp-conf.js 文件，配置appKey, appVersion.

```
// utils/hotapp-conf.js
exports.hotAppKey='此处填写您在HotApp小程序统计后台中显示的App Key'; //小程序在zhima平台注册的appKey
exports.appVer='0.1.0';     //本地小程序的版本号,用来区分错误统计
```

3、 接入统计SDK

```
//app.js
var hotapp = require('utils/hotapp.js');
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

统计接入成功后 会自动统计、今日启动数、昨日启动数、今日新增用户、昨日新增用户、今日活跃、昨日活跃数和今日累计用户等数据。



