### HotApp微信登录

什么是微信登录?  
通过微信登录后的, 可获取到用户的openid，针对单个小程序的openid是固定的。 通过HotApp小程序统计的微信登录功能，您只需要一行代码就可以接入微信登录  
\(1\) 在HotApp小程序统计的后台设置微信小程序的APPID 和 AppSecret  
\(2\) 通过一行代码获取到使用小程序的用户的openid

```
// 可以通过回调函数来使用openid
hotapp.wxlogin(function(openID){
    console.log(openID);
});

// 也可以登录之后再来获取openid
hotapp.wxlogin();
...
var openid = hotapp.getOpenID();

// 如果您没有在后台设置APPID和AppSecret或者设置得不正确,
// 那么这时获取的是我们生成的一个id, 我们称这个id为FakeOpenID
// 您可以通过这个id来标识一个用户, 但是用户清空缓存或者更换设备, 那么此uuid是无效的
hotapp.wxlogin(function(fakeOpenID) {
    console.log(fakeOpenID);
});

// 登录之后再来获取openid
hotapp.wxlogin();
...
var fakeOpenID = hotapp.getFakeOpenID();
```



