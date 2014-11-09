# Modernist

> Theme for [Hexo]. Based on [modernist theme] for GitHub Pages.

[Demo the Theme]


#基于原版做过哪些修改？

- 修改了部分字体大小，使模版更适合显示中文。
- [提速]将jquery、html5shiv CDN 更换为国内地址（原因你懂）
- [提速]将css中载入的google字体文件转移到本地。
- 增加返回顶部、快速评论按钮
- 增加 分类、标签云、最新文章 3个widgets。
- 增加是否将widgets右置选项
- 增加分享功能（仅添加了QQ，感觉其他的没什么实际用处）
- 增加百度统计（配置中开启百度统计，并将统计代码粘贴在modernist\layout\_partial\baidu-tongji.ejs 中。注：请使用“百度统计异步代码”）原有google被保留，您也可以使用。
- 增加多说评论功能。


## 安装

```
git clone git@github.com:guan6/hexo-modernist.git themes/modernist
```

## 启用主题

编辑 “_config.yml”文件，将theme项修改为：modernist

## 升级

```
cd themes/modernist
git pull
```

## 配置

``` yaml
# Header
menu:
  Home: /
  Archives: /archives
rss: /atom.xml

# Content
archive_date_format: MMM DD
fancybox: true

# widgets
widgets:
- category
- tagcloud
- recent_posts

# widgets right
widgets_pos_right: true

# share
share:
  enable: false
  qq: false

# gotop
gotop:
  enable: true
  soll_top: 350
  speed: 800

# Comment Plugin
duoshuo_shortname: 

# Miscellaneous
google_analytics:
baidu_tongji: false
favicon: /favicon.ico
```

- **menu** - 博客导航设置
- **rss** - RSS link
- **archive_date_format** - 归档页面时间格式.
- **fancybox** - Enable [Fancybox]
- **widgets** - 部件
	- **category** - 分类
	- **tagcloud** - 标签云
	- **recent_posts** - 最新文章
- **widgets_pos_right** - true 开启widgets右置，设置为空或false，widgets在底部
- **share** - 分享
	- **enable** - 是否开启
	- **qq** - qq分享
- **gotop** - 返回顶部
	- **enable** - 是否开启
	- **soll_top** - 滚动多少像素显示按钮
	- **speed** - 页面滚动速度
- **duoshuo_shortname** - [Duoshuo] 多说ID
- **google_analytics** - Google Analytics ID
- **baidu_tongji** - 百度统计
- **favicon** - Favicon path

[Hexo]: http://zespia.tw/hexo/
[modernist theme]: https://github.com/orderedlist/modernist
[Demo the Theme]: http://blog.dafengning.com/
[Duoshuo]: http://duoshuo.com
[Fancybox]: http://fancyapps.com/fancybox/