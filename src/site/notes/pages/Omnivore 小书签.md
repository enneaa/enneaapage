---
{"dg-publish":true,"permalink":"/pages/Omnivore 小书签/","noteIcon":"1","created":"2023-07-19T16:54:07.298+08:00","updated":""}
---

[[pages/文稿\|文稿]]
Omnivore是一款稍后读应用，用法可以参考： [[pages/使用Omnivore实现渐进式阅读\|使用Omnivore实现渐进式阅读]]。
官方提供了浏览器扩展或者分享到应用程序来保存链接，不过有的时候用小书签保存链接更为方便，因为手机浏览器大部分安装不了扩展，Omnivore网页端也足够好用，没必要再装个APP。
把下面的链接保存为书签，或者拖到书签栏。
[RTL](javascript:location.href='https://omnivore.app/api/save?url=%27+escape(location.href)
直接点击小书签，或者在地址栏输入 `RTL` 搜索再选中小书签，即可将当前网页保存到Omnivore。

小书签代码：
```
javascript:location.href='https://omnivore.app/api/save?url=%27+escape(location.href)
```