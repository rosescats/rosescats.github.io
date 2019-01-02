---
title: 影印 PDF 文檔分割
date: 2015-01-04
tags: PDF分割
categories: 技术
---

## 爲什麼會尋找這些工具？

2014寒假某天，我收到一封 email ，某人找我抽空幫忙下載「[古本金瓶梅一百回](http://hong.ioc.u-tokyo.ac.jp/list.php?p=68&order=rn_no&jump_data=&nsukey=XlHf2AkpVttaVboGKOW5TNfjklZHIGoZg5hyBszWfVMXh35S5yLbNXlAKUp9f6r7b2clq%2FtCZN8Y4Ybnz29XBw%3D%3D)」，有時間再處理成單頁單面 PDF 。進入網站傻眼了，600+ 個影印 pdf （其实是一堆 jpg ），先 google 了一些批量下載方法，最終用 wget 命令勉強完成了下載工作（關於 wget 批量下載，下次再細談）。每個文檔都類似這樣：

![金瓶梅](https://36.media.tumblr.com/0b98adf8dc6ecae7c4ae9da1f724b0b7/tumblr_nnkpxoyM2z1t03x8ro1_1280.jpg)

我將600多個 jpg 合併爲兩個 pdf 文檔後，開始尋找合適的分割工具。
（事後回想，我完全可以批量分割後再合併爲 pdf ，豈不更快？）

## 找到的相關工具

**1、[a-pdf page cut](http://www.a-pdf.com/faq/how-to-split-pdf-pages-in-half.htm)**

可批量處理 split pdf pages in half ，操作運行速度較快，也有人認爲其相當於將另一半遮擋處理。

適用平臺：windows

需要注意的是，很多中文古籍原文爲右起翻頁，而此工具處理後默認從左文檔起排列。因此，需要先將待分割內容整體逆時針旋轉九十度，再分割，最後順時針旋轉九十度。

官方網頁有具體操作 step 解釋。

經過若干次對比，我選擇了這個工具。

### 2、adobe acrobat

adobe acrobat （不是 adobe reader）是 adobe 系列產品之一，官方有試用版本，其「打印」功能可通過設置「平鋪百分比」達到「分割」效果。

手動調節百分比時可以看到右側預覽效果，使得分割線與影印文檔中線接近即可。

缺點：adobe acrobat 一次操作太多，會很慢，甚至電腦卡機。（如果你的電腦優化不行或很容易死機，在處理時通過設置處理頁面號碼，多次操作）

對古籍分割不友好，分割後，原來的兩面一頁前後順序顛倒。我開始用這個工具分割上面的影印古籍時，就被坑得挺慘。我天真地以爲先將原文檔旋轉一次，再分割會達到預期效果，但它是個「死腦筋」，還是順序顛倒。

[**操作方法**](http://www.penddy.com/how-to-cut-double-sided-page-of-the-pdf-into-a-page.html)

關於 acrobat 插件「海森堡」，我已無力常識，有時間再折騰。

### 3、PyPDF2

準備：

a.用到 python 的 [pypdf2](https://github.com/mstamy2/PyPDF2) 庫，下載後解壓縮進入文件夾，使用命令 **`python setup.py install`** 將該模塊裝入系統。

b.下載腳本文件[c2s](http://alex4814.in/ac/wp-content/uploads/2014/08/c2s.tar.gz)，用 **`chmod +x c2s`** 修改其權限可執行。

使用：
先 **`cd`** 到待處理文件所在地址，再**`./c2s  dst.pdf`** 執行（src.pdf 是待處理文件的名稱，dst.pdf 是處理後新文件名稱）

要求： mac 平臺；Python 2.7.8

*問題：python 在 linux 應該可以執行的，但我如此執行後的新文件都無法打開，查看文件內無字節。難道是因爲我的 python 版本是2.7.6原因？*


[**原鏈接**](http://alex4814.in/ac/archives/638)

### 4、scantailor

*基於 C++ 的跨平臺工具，用來處理圖片 pdf ，可以切分掃描頁、傾斜校正、邊框修正。*

**4.1安裝使用**

window 系統中直接下載該工具安裝使用。

ubuntu 系統中安裝：
前期準備：scantailor 運行環境需要，安裝如下：

libjpeg: **`apt-get install libjpeg62-dev`** (any -v)

zlib: **`apt-get install zlib1g-dev`**      (any -v)

libpng: **`apt-get install libpng12-dev`**   (any -v)

libtiff: **`apt-get install libtiff4-dev`**  (any -v)

libboost: **`apt-get install libboost1.55-all-dev`** (>=1.35 -v，經安裝測試，1.40安裝失敗)

libxrender: **`apt-get install libxrender-dev`**  (any -v)

cmake: **`apt-get install cmake`**

**安裝時都不能出現 error 提醒，否則後面無法安裝**

**4.2安裝 scantailor**

cd 到 scantailor 文件夾，執行 **`cmake .`**，以 **`- configuring done`** 結束,
繼續 **`make`** and **`sudo make install`**

**4.3打開 scantailor**
 **`alt+F2`** ,輸入 scantailor 運行會看到如下界面：

![scantailor](https://40.media.tumblr.com/65bb014af7318cc54903fd8651630af9/tumblr_ntzh1qixvh1uft3xho1_540.png)

[**操作視頻**](https://vimeo.com/12524529)

[**scantailor 下載**](https://github.com/scantailor/scantailor/releases/tag/RELEASE_0_9_11_1)

[**三個平臺安裝教程**](https://40.media.tumblr.com/65bb014af7318cc54903fd8651630af9/tumblr_ntzh1qixvh1uft3xho1_540.png)
