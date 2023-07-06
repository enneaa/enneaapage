---
{"dg-publish":true,"permalink":"/pages/Logseq 和 Obsidian 联用的可行方式/","noteIcon":"1","created":"2023-07-06T11:46:07.971+08:00","updated":""}
---


Obsidian&Logseq都是基于本地markdown文件，这奠定了两者联用的基础。
Obsidian 是文档型双链笔记，基本单元是页面，Logseq 是大纲型双链笔记，基本单元是块。使用上以obsidian兼容logseq为主，把logseq视为obsidian的一个插件，进行大纲编辑和任务管理，obsidian作为笔记浏览器和信息集散中心，文档撰写还是使用obsidian。
具体而言，由于logseq抛弃了文件夹管理，并将笔记全部存放在pages文件夹下，把logseq日志笔记的存储位置也统一为pages文件夹。在obsidian中将所有笔记文件放在pages文件夹中，也放弃文件夹关联，两者共用一个笔记库。在obsidian中常用的页面添加为书签，用书签来管理，在logseq中常见的页面添加到收藏。在obsidian中启用日记插件和日历插件，点击日历插件打开/新建当日日志并输入内容，在logseq中在日志页面上输入内容，两者都使用日志记录流程，共用日志笔记文件。
尽量减少块引用的使用，双链主要使用页面引用，保持兼容性。


---
### 关于Obsidian&Logseq的一些零散想法

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/pages/obsidian-and-logseq/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





- @ [[pages/Obsidian\|Obsidian]] @ [[pages/Logseq\|Logseq]]
- [[pages/Obsidian\|Obsidian]] 是一个基于 [[pages/Markdown\|Markdown]] 的操作系统。在功能实现上，可以认为 Logseq 是 Obsidian 的一个插件。
- Obsidian 是大海，Logseq 是江河。
- 一个是列表项为基本单元，一个页面为基本单元。
- [[pages/大纲笔记\|大纲笔记]]适合灵活组织列表项之间的从属关系，[[pages/文档笔记\|文档笔记]]则需要用各级标题来切分。
- 再一个区别在于，一个打通了反向链接面板和正文，反向链接直接从属于当前节点，另外一个由于以文档为基本单元，只显示了反链内容而没有打通，需要点击打开新页面进行编辑。
- 一个更结构化，一个更自由兼容。
- Logseq 是条目笔记，Obsidian 是卡片笔记，
- 一个钩子🪝是条目，一个钩子🪝是标题。
- 在实际使用中，可以把 Logseq 作为大纲编辑器，Obsidian 用来管理笔记库。
- 最大的区别是链接的基本单元的不同，一个是页面一个是条目。在 Logseq 中，页面不过是条目的另一种形态。
- 如果在 Logseq 的使用中克制对条目引用的使用，则两者是兼容的。
- 个人认为链接到页面足够了。 ^590d24
	- 在大部分情况下 Logseq 的还是链接到页面居多。
	- 如果一个内容需要链接，那么就足以建立一个页面用来链接了。
	- 链接到条目需要给条目编码，这有违 Markdown 的可读性、可编辑性。链接到页面只需在框内输入页面名称。链接到条目则需在软件索引的帮助下选中对应内容，并生成一串个人无法辩识编辑的编码。
	- 页面引用是全库通用，条目引用只限于原处，除非将条目设为页面引用。^28b3df
- obsidian 作为信息集散地。
- [[pages/文档笔记\|文档笔记]]可以包容[[pages/大纲笔记\|大纲笔记]]。
- obsidian 是军火库，logseq 是机关枪。
- 使用习惯兼容logseq，格式兼容obsidian。

</div></div>
