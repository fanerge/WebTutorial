#	SEO
##	HTML文档编码
###	document#title
The title should ideally be less than 64 characters in length.[W3C-TITLE](https://www.w3.org/Provider/Style/TITLE.html)
###	meta#keywords
You describe the Web page's keywords in the content attribute.
`<meta name="keywords" content="W3C, HTML, HTML5, XHTML, CSS, CSS3, SVG, MathML, WCAG">`
###	meta#description
You describe the Web page's description in the content attribute.
`<meta name="description" content="The World Wide Web Consortium (W3C) is an international community where Member organizations, a full-time staff, and the public work together to develop Web standards.">`
##	PC和Mobile页面互相指引
```
<link rel="alternate" media="only screen and (max-width: 640px)" href=“{WAP版对应URL}" />
<link rel="canonical" href="{PC版对应URL}" />
```
##	Universal Link
##	页面微信息结构化
对详情页标签打itemscope、itemtype、itemprop
##	图片SEO
每张图片，尽量加上 alt和title属性
PS:搜索关键字后点击图片可以查看到对应网址
##	Sitemap
changefreq:页面内容更新频率
lastmod:页面最后修改时间
loc:页面永久链接地址
priority:相对于其他页面的优先权
url:相对于前4个标签的父标签
urlset:相对于前5个标签的父标签
##	robots协议
User-agent: * 这里的*代表的所有的搜索引擎种类，*是一个通配符
Disallow: /ab 禁止爬取ab文件夹的所有目录及文件
Allow: /cgi　这里定义是允许爬寻cgi目录下面所有目录及文件
Sitemap: 网站地图，告诉爬虫这个页面是网站地图


#	HTTPS升级
HTTPS中所有HTTP自动替换为HTTPS，需添加响应头。
Content-Security-Policy: upgrade-insecure-requests
or
html中添加meta
`<meta http-equiv="Content-Security-Policy" content="upgrade-insecure-requests">`

