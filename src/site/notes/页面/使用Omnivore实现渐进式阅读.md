---
{"dg-publish":true,"dg-path":"PAGE/使用Omnivore实现渐进式阅读.md","permalink":"/PAGE/使用Omnivore实现渐进式阅读/","noteIcon":"1","created":"2023-05-24T08:46:09.843+08:00","updated":""}
---


Omnivore 是一款新兴的稍后读应用，可以认为就是另一款 Pocket ，不过 Pocket 现在高亮标注一篇文章只能有三处，超过就要会员了，Omnivore 现在使用完全免费，保存文章后，可以进行标注、批注，并导入至 Obsidian。

### 使用 Omnivore 进行阅读
Omnivore 的网址是 [Omnivore](https://omnivore.app/home)，中文使用文档在这，[Omnivore 使用文档](https://docs.omnivore.app/zh/)。
使用非常简单，打开官网，注册账号，在网页里即可添加需要保存的文章链接，还可以安装浏览器扩展进行保存。
阅读文章时，选中文字，点击页面下部的 highlight 即可高亮文字，点击 note 即可对高亮内容添加笔记。
![使用 Omnivore 实现渐进式阅读_1.jpg|150](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_1.jpg)![使用 Omnivore 实现渐进式阅读_2.jpg|150](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_2.jpg)
点击阅读文章界面右上角的笔记按钮，即可对整篇文章添加笔记。
![使用 Omnivore 实现渐进式阅读_4.jpg|150](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_4.jpg) ![使用 Omnivore 实现渐进式阅读_3.jpg|150](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_3.jpg)

### 将笔记内容同步至 Obsidian
首先在 Obsidian 插件库中搜索 Omnivore 安装插件。
打开 Omnivore 插件设置：
![使用 Omnivore 实现渐进式阅读_6.jpg|150](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_6.jpg) ![使用 Omnivore 实现渐进式阅读_7.jpg|150](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_7.jpg)
点击 https://omnivore.app/settings/api ，获取 API key，并粘贴到插件设置里。
在下面 Template 栏中输入以下内容：
```
{{#labels.length}}{{#labels}} #{{{name}}}{{/labels}}{{/labels.length}}
来源:: [{{{title}}}]({{{originalUrl}}}) [⤴️]({{{omnivoreUrl}}})  [[资讯]] 

{{#note}} 
#### 全文批注
- 💡{{{note}}}{{/note}}

#### 高亮批注
{{#highlights.length}}
{{#highlights}}
- {{{text}}} {{#labels}} #{{name}} {{/labels}} 
{{#note}}  - 💡{{{note}}}{{/note}}
{{/highlights}}
{{/highlights.length}}
```
![使用 Omnivore 实现渐进式阅读_8.jpg|200](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_8.jpg)
再往下设置导入笔记的存储路径等等：
![使用 Omnivore 实现渐进式阅读_9.jpg|200](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_9.jpg)

好啦😊
现在点击 Omnivore 按钮，就会自动将高亮和笔记导入到 [[页面/Obsidian\|Obsidian]] 中来。
![使用 Omnivore 实现渐进式阅读_10.jpg](/img/user/%E5%85%B6%E4%BB%96/%E9%99%84%E4%BB%B6/%E4%BD%BF%E7%94%A8%20Omnivore%20%E5%AE%9E%E7%8E%B0%E6%B8%90%E8%BF%9B%E5%BC%8F%E9%98%85%E8%AF%BB_10.jpg)

在 Obsidian 中可以对笔记进一步整理总结，实现渐进式阅读。

### 什么是渐进式阅读
简单来讲就是按照以下步骤分层分步进行摘要、总结、分析。
第一层：原文摘要，指的是将原文中重要的信息摘录到笔记中。
第二层：重点摘要，在第一层基础上，对其中更为核心的观点或关键词进行「加粗」处理。
第三层：高亮摘要，在第一二层基础上，对一些重点段落进行「高亮」处理，突出文章的主旨。
第四层：总结，「用自己的话」去描述和概括对当前笔记的理解。
从下往上开始：
- 50% 左右的信息无任何笔记
- 25% 标粗进入第二层
- 20% 能被高亮
- 只有 5% 才会再次总结
- 只有 1% 的内容，能进入第五层的融合，因为这需要大量的时间和精力。

1. [何为渐进式总结](https://www.notion.so/3a8c5d77b5be42c58719d174bfbfa935)
2. [玩转 Obsidian 06：如何用渐进式总结笔记，把知识交给未来的自己 - 少数派](https://sspai.com/post/69025)