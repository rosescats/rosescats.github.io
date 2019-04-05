---

layout: post

title: XMind ZEN 隐藏导出水印的方法

categories: 技术

tags: 'XMind ZEN'

date: 2019-04-05

---

[XMind ZEN](https://www.xmind.net) 是继 XMind8 新出的思维导图绘制工具，两者功能差不多。

如果不考虑模板，一直使用免费版就足够了，但导出图片、PDF会自带背景水印。

下面讲解如何在不使用第三方奇奇怪怪的破解软件的情况下，如何去掉/隐藏水印。

> 系统：Ubuntu
>
> 软件版本：XMind ZEN 9.0.3
>
> 语言环境：English

### 第一步：下载安装 XMind ZEN

不多说，从 XMind 官网下载：https://www.xmind.net/download/

### 第二步：修改水印文件

XMind ZEN 在 Ubuntu 默认安装在了目录 `/opt/XMind ZEN/`，水印文件在 `/opt/XMind ZEN/resources/app/out/imgs` 目录下面，文件格式是 `.svg`。

对应导出PNG图片、PDF、打印，需要修改的文件有：

1. `pdf-footer-en-US.svg`
2.  `png-watermark-en-US.svg`
3. `print-watermark-en-US.svg`

前两个文件用 `gedit` 编辑打开，删除所有内容并保存。

print 水印文件用 `gedit` 打开编辑，修改 `opacity=0.2` 参数，改为 `0`，就是全透明了，隐藏水印。

如果系统语言是中文简体，则分别修改结尾是 `zh-CN` 的文件。

![儿童教育学科体系](https://i.loli.net/2019/04/05/5ca74f8a553fd.png)
