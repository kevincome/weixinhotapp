# 客服API

通过客服API可以自由灵活的设置客服回复的内容和类型，目前主要有下面三种回复类型：

（注意：sesion-from最大字符串长度为1024，超过1024会被截取，导致json出错）



**文字回复**

```
<button open-type='contact' session-from='{"title":"您好，有什么可以帮助您的"}'>自动回复标题</button>
```



**网址回复**

```
  <button open-type='contact' session-from='{"title":"打开官网","url":"http://xiaokefu.hotapp.cn "}'>自动回复打开网址</button>
```



**图文回复**

```
   <button open-type='contact' session-from='{"title":"点击关注",“url”:“mp.weixin.qq.com ","desc":"关注【微生成】公众号，解锁更多功能","img":“http://qq.com/test-not-found-img.png ”

   }'>图文消息，关注我们</button>
```



