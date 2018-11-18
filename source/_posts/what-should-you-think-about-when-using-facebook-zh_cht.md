---
title: 使用 Facebook 時，應該考慮什么？
top: 0
date: 2018-11-03
updated: 2018-11-03
tags: 隐私安全
categories: translation
---

> 原文：[https://veekaybee.github.io/2017/02/01/facebook-is-collecting-this/](https://veekaybee.github.io/2017/02/01/facebook-is-collecting-this/)

![winnower.jpg](https://i.loli.net/2018/08/31/5b8931e1c585a.jpg)
**Courbet, The Winnowers**

摘要：Facebook 通過眾多渠道使用數百種方法收集有關你的數據。你很難退出，但通過了解他們收集的內容，可以認識到 Facebook 平台的危險性，并選擇以更嚴格的限制來使用 Facebook.

目錄：
* [Facebook 如何收集數據](#Facebook如何收集數據)
* [在你發布之前，Facebook 知道什么](#在你發布之前，Facebook知道什么)
* [發帖之后：Facebook 收集有關你的內容](#發帖之后：Facebook收集有關你的內容)
* [Facebook 內部用你的數據做了什么](#Facebook內部用你的數據做了什么)
    * [影子檔案](#影子檔案)
* [Facebook 和 營銷商是什么關系](#Facebook和營銷商是什么關系)
* [Facebook 向政府提供哪些數據](#Facebook向政府提供哪些數據)
* [你退出 Facebook , Facebook 會跟蹤什么](#退出Facebook后，Facebook會跟蹤什么)
* [當我使用 Facebook 時，應該考慮什么？](#當我使用Facebook時，應該考慮什么？)
* [如果我不想讓 Facebook 獲取我的數據，應該怎樣做？](#如果我不想讓Facebook獲取我的數據，應該怎樣做？)

Facebook 無論好壞，已經成為我們的網絡客廳、[第三空間](https://en.wikipedia.org/wiki/Third_place)。這是我們與好友交談、發布新聞、組織活動、悼念逝者、慶祝嬰兒出生、訂婚、找新工作、展示新發型和假期的地方。

Facebook 平台已經占據了如此大的占有率，并且開始作為我們的[冥想盆](http://harrypotter.wikia.com/wiki/Pensieve)。因此，了解 Facebook 公司獲取使用我們的希望、夢想、政治宣言、嬰兒照片信息做什么尤為重要。

從獲取數據開始。2014年，Facebook 工程師寫到他們[每天可以獲取大約 600TB 的數據](https://code.facebook.com/posts/229861827208629/scaling-the-facebook-data-warehouse-to-300-pb/)。

對比一下，《戰爭與和平》的文本大小是3.1MB；1966年的蘇聯版《戰爭與和平》電影時長7小時，大小是[8GB](https://www.reddit.com/r/iphone/comments/462isr/get_some_storage_back_by_trying_to_download_a/)。

因此，人們每天上傳的數據總量相當於1.93億本《戰爭與和平》書籍、75,000部《戰爭與和平》電影。

[Facebook 數據政策](https://www.facebook.com/policy.php) 概述了它收集的內容和如何處理數據。然而，和大多數公司一樣，Facebook 忽視了實際要點，沒有告訴用戶到底發生會什么。

我揣測自己寫每條狀態更新時的按鍵，使我感到沮喪，對此決定做一些研究。以下所有信息來自科技商業新聞報導、學朮出版物、我作為 Facebook 用戶能夠在客戶端看到的內容。作為一名從事用戶數據工作10年以上的專家，我在這篇文章中加入了自己的詮釋。

如果任何一位 Facebook 員工想要對此篇文章進行糾正，我會很樂意聽他們說并沒有像下文所說的那樣收集和處理用戶數據。

## Facebook 如何收集數據

為了理解 Facebook 數據收集的工作原理，我繪制了一個（非常非常）簡單的圖表。用戶將數據輸入用戶界面（應用程序），這是前端。

這些數據隨后被收集到 Facebook 的數據庫（這些數據庫有很多），這是后台。

用戶在前端看到的數據是后台數據的子集。

![facebookui.png](https://i.loli.net/2018/08/31/5b89330d60b19.png)

如果你對更多的技朮規格感興趣，Google 上面有很多架搆圖。Facebook 正處在處理大數據的前沿，它們的堆棧包括 Hive, Hadoop, HBase, BigPipe, MySQL, Memcached, Thrift 更多。所有這些都存放在許多大型數據中心，比如 Prineville Oregon 數據中心。

## 在發帖之前，Facebook 知道什么？

> 在點擊"post"之前，Facebook 可能就開始收集數據了。當你編輯信息時，[Facebook 開始收集你的按鍵內容](http://www.slate.com/articles/technology/future_tense/2013/12/facebook_self_censorship_what_happens_to_the_posts_you_don_t_publish.html)。

Facebook [曾經使用這些數據來研究自我審查](http://www.aaai.org/ocs/index.php/ICWSM/ICWSM13/paper/viewFile/6093/6350)（研究報告 PDF）。

![prepost.png](https://i.loli.net/2018/08/31/5b89330ce3682.png)

研究員寫道：

> 我們報告的結果來自一份探索性分析，檢查 Facebook 「最后時刻」的自我審查，或者在寫完后在 Facebook 被過濾的內容。我們在 17 天內收集了 390萬名用戶的數據，并將自我審查行為與用戶描述、用戶社交圖表以及他們之間的互動特徵聯系起來。

這意味着，如果你發布了類似於「我只是討厭我的老板，他把我逼瘋了。」這樣的內容。雖然在最后一刻刪除了這句話，改寫為「伙計，現在的工作真是太瘋狂了」，Facebook 仍然知道你在刪除之前輸入的內容。

以下是他們用於研究的數據點：

![prethought.png](https://i.loli.net/2018/08/31/5b89330d1426a.png)

這里值得注意的是：就像不能確保未發布的內容不會被存儲；用戶刪除帖子、評論和簽到，不能確保數據真的被刪除了。

因此，即使刪除了帖子，Facebook 仍記錄了它。Facebook 記錄[元數據](http://www.ruanyifeng.com/blog/2007/03/metadata.html)，或記錄有關你的數據的數據。比如，撥打電話的數據就是實際談話內容，它的元數據是撥打電話的時間、地點和時長等信息。

對於 Facebook 來說，元數據和真實數據同等重要，它使用元數據推斷你的身份。在 Chrome 瀏覽器使用開發者工具，可以相對容易地看到大量數據通過 xhr 從你的客戶端傳送到 Facebook 后端。我不是一個前端忍者（但實際上我很樂意和其中一位談話，看看我們還能做些什么），但從一張圖上，可以看到 Facebook 在追蹤用戶做某件事花費的時間嗎？具體內容不確定，但它可能計算出了耗費在 Facebook 網站的時間。[Facebook 報道說](https://www.nytimes.com/2016/05/06/business/facebook-bends-the-rules-of-audience-engagement-to-its-advantage.html?_r=0)。

![xhr-fb.png](https://i.loli.net/2018/08/31/5b89330d36265.png)

順便說一句，對於賬戶刪除也是如此。

由於 Facebook 擁有如此多的系統和可以數據共混的地方，正如一位 Facebook 前顧問所寫：

> 回答你提問的第一部分，「你可以付錢讓 Facebook 徹底刪除你的所有信息嗎？」假設「徹底」意味着完全清除你留在 Facebook 的任何痕跡。答案是不會。

同樣，如果刪除帖子，并不能確保 Facebook 不會在后台數據庫保存這個帖子，它只是不會顯示在客戶端頁面。

只要你真的寫了帖子、上傳了圖片，或是修改了任何信息，對於 Facebook 內部研究使用、轉售給 Acxiom 這樣的營銷聚合商、[通過國家安全局這樣的機搆](http://www.nytimes.com/2013/09/29/us/nsa-examines-social-networks-of-us-citizens.html)和 NSA 的稜鏡計划提供給美國政府，這一切都是絕對公平的游戲。

## 發帖之后：Facebook 收集關於你的什么數據

很顯然，Facebook 收集你自願提供給它們的所有數據：政治派別、工作地點、最喜歡的電影、最愛讀的書、打卡簽到的位置、評論、對帖子的任何所有反應。Facebook [允許你下載他們的數據庫中關於你的數據子集](https://www.facebook.com/help/302796099745838)。

在我個人的數據子集中，我可以看到：

* 我上傳的照片、標記了我的照片
* 視頻
* 我曾經發布在自己時間線上的一切內容（包括我表示感興趣的事情、人們發布在我的時間軸上的內容、共享的記憶）
* 好友、添加我為他們的好友
* 我的所有私人信息
* 我參加過的活動
* 我登錄過的每一台設備

以及，我可能感興趣的廣告。這不是我自己寫的東西，而是 Facebook 基於我發布的每條內容，利用算法生成的。

我們將會在廣告部分討論這個問題。

除了數據和元數據，Facebook 也跟蹤用戶的意圖。上面已經探討了其中一種跟蹤方式：未發布的信息，另一種則是在視頻中的[熱圖跟蹤](https://techcrunch.com/2016/08/10/360-storytelling/)。

Facebook不僅知道關於你的一切信息，也了解你的朋友關系。一言以蔽之，Facebook 很了解你，盡管你沒有完整填寫你的個人資料、也沒有主動發布到網站。

## Facebook 內部用你的數據做了什么？

Facebook 利用收集到的數據做了很多事情。

首先，Facebook 對信息進行簡單查詢用於提高網站性能或用於行業報告（例如，網站運行時間，[Facebook 用戶數量](http://veekaybee.github.io/how-many-users-do-you-have/)，今天的廣告收入是多少？）。這對於任何公司都是如此。

不過，對於 Facebook 來說有所轉變。Facebook 有一個完整的工程團隊致力於搭建工具，使得數據更易於用 SQL——類似基於 Hadoop 和 [Hive](https://www.facebook.com/notes/facebook-engineering/hive-a-petabyte-scale-data-warehouse-using-hadoop/89508453919/) 的語言——查詢。盡管 Facebook 聲稱嚴格控制權限，有些用戶卻并[不這么認為](http://www.techtimes.com/articles/36186/20150227/who-access-account-details-facebook.htm#sthash.GXFknTxA.dpuf)。

> 唱片公司 Anjunabeats 主管 Paavo Siljamäki 在 Facebook 發帖提醒人們注意這個問題，訪問該公司洛杉磯辦事處時，可以很容易訪問他的 Facebook 賬戶而無需他的密碼。

這里是[ Facebook 員工訪問私人數據的賬戶的更多說明](https://www.quora.com/Do-Mark-Zuckerberg-or-Facebook-employees-have-a-skeleton-key-granting-them-access-to-every-members-Facebook-profile-page-and-information)。

其次，Facebook 把用戶作為實驗對象進行學朮研究。在數據政策中沒有提到這一點，這很有意思， [Facebook Research 主頁](https://research.fb.com/)的標題寫着：「在 Facebook, 研究滲透到我們所做的一切。」

Facebook 有一個相當大的數據科學團隊（[最新統計是 41 人](https://research.fb.com/people/page/3/?cat=6)）。我想說的是，一個擁有 15000 人同樣規模的公司，如果它真的想要積極推動一個數據科學研究項目，可能只有 5 個數據科學家。

然而，直到 2014 年為止，還沒有任何程序可以檢查被訪問的數據類型、以及進行怎樣的研究。正如一位[前 Facebook 數據科學家寫到](http://andrewledvina.com/code/2014/07/04/10-ways-facebook-is-the-devil.html)：

> 我在 Facebook 的時候，沒有一個機搆審查委員會來審查為內部目的進行實驗的決定。一旦有人得出結論，他們決定要把這篇文章發表到雜志上，那么在可發表的內容上，確實存在反反復復的公共關系和法律問題。如果你想做一個實驗，看看人們會點擊綠色按鈕還是藍色按鈕，你無需得到批准。同樣，如果要測試新的廣告定位系統，以查看用戶是否點擊了更多廣告，是否收入增加，無需獲得機搆批准。

雖然他接着指出這在大多數以軟件服務的公司中是正常的，但大多數 SaaS 公司在過去十多年中也沒有精心收集人們生活中最私密的細節。

他繼續說道：

> 大多數人在 Facebook 研究數據的基本目的是影響和改變人們的情緒和行為。他們一直在做這件事，讓你更喜歡故事，點擊更多的廣告，花費更多時間在 Facebook 網站。

盡管這是大多數網站的目標，但每天[花費超過 40 分鐘](http://www.businessinsider.com/how-much-time-people-spend-on-facebook-per-day-2015-7) 在企圖在情感上削弱你的網站上，你可能需要三思而后行。

Facebook 除了挖掘文本內容、[研究我們的情緒](https://research.fb.com/support-when-you-re-feeling-blue/)，它還會[操縱它們](https://www.theguardian.com/technology/2014/jun/29/facebook-users-emotions-news-feeds)。

新聞 Feed 是操作的首選。特別是因為 Facebook 已經設計出盡可能吸引人的功能：它是我們神經系統的突觸糖。Facebook 希望確保你[盡可能在 Feed ](http://newsroom.fb.com/news/2015/06/news-feed-fyi-taking-into-account-time-spent-on-stories/)多花時間，并為此花[更多時間來處理嬰兒照片](https://www.wired.com/2014/04/babies-on-facebook/)和其它快樂的事情，以及那些引發爭議和憤怒的新聞。而像「我今天吃過早餐」這樣的正常狀態不會引起任何反應。

這就是當今所謂過濾氣泡是怎樣興起的。因為人們會點一些他們感興趣的東西，所以 Facebook 就只呈現吸引用戶的內容，這意味着其他觀點、朋友和圖片會從一個人的 Facebook Feed 中刪除。如果想了解這種方式是如何工作的，可以參考 [Red Feed、Blue Feed](http://graphics.wsj.com/blue-feed-red-feed/), 展示了自由與保守的 Facebook Feed 的不同之處。

他們還在研究其它什么？首先是[同性戀出櫃](gay)比例。Facebook 如何知道這些的？「在過去的一年里，大約有 80 萬美國人更新他們的個人資料，表達同性吸引或專屬性別」。

大量的 Facebook 研究都是關於圖論，也就是我們和朋友間的關系圖。換句話說，它正在對從未同意的學科進行人類學研究。

例如在近期，數據科學小組發表了一項關於[美國移民社區的社會關系](https://research.fb.com/publications/the-social-ties-of-immigrant-communities-in-the-united-states/)的研究。在報告中，研究員使用了以下數據：

> 我們將我們的分析限制在基於已經被確認的社交網絡數據基礎上的綜合判斷，這些人在分析前 30 天內至少使用過一次 Facebook. 我們使用個人資料中指定的家鄉來確定用戶的國籍。

> 此外，我們也把分析限制在目前至少有2個朋友居住在本國的人和目前居中在美國的另外 2 個朋友。我們的結果基於超過 1000 萬滿足這些標准的人的樣本。整篇報告中，所有關於 Facebook 用戶的引用都毋庸置疑地暗示了這些限制。

這些是我們知道的公開研究，他們還在做哪些非公開的研究？

Facebook 理所當然喜歡研究的另一個內容是[人臉](https://www.bloomberg.com/news/articles/2016-10-26/is-facebook-s-facial-scanning-technology-invading-your-privacy-rights)。每次你在照片中標記自己時，Facebook 會認出你，并且做相應調整。

> Facebook 鼓勵用戶在他們個人帖子中上傳的照片中「標記」人，社交網絡將收集到的信息儲存起來。Facebook 使用一個叫作 DeepFace 的程序來匹配用戶的其它照片。

![selfie.png](https://i.loli.net/2018/08/31/5b89330d3ab7e.png)

這個名為 DeepFace 的程序是獲取更多准確標簽的絕佳方式。它也是侵犯個人隱私的絕佳手段。比如，倘若你不想被標記該怎么辦？假如你在政府抗議活動中？或者簡單來說，如果你和一位朋友去聽音樂會，不是和另一位朋友，卻還不想讓對方知道，該怎么辦？

不幸的是，很快就沒有隱私可言了。Facebook 正致力於[識別照片中人的身份](http://fortune.com/2015/06/23/facebook-facial-recognition/)。Facebook 上[關於 DeepFace 的論文](https://www.cs.toronto.edu/~ranzato/publications/taigman_cvpr14.pdf)指出，「人臉識別技朮對社會和文化影響是深遠的」，然而根本沒有談到人臉被標記的可能的隱私危險。[比如](http://spectrum.ieee.org/biomedical/imaging/facebooks-face-recognition-tech-goes-on-trial)：

 > 她說，『我們很快就會在商店里安裝攝像頭，以識別顧客的購物情況』。

他們怎么知道這些的？

因為這些數據是我們自願提供的。每次更新狀態、上傳照片并做標記、給朋友發信息、在一個地方簽到、登錄 Facebook, 系統都會自動生成一條信息保存到數據庫中——「嘿，這個人現在在Facebook 世界里。」，包括了 [Whatsapp](https://techcrunch.com/2016/08/25/whatsapp-to-share-user-data-with-facebook-for-ad-targeting-heres-how-to-opt-out/) 和 [Instagram](https://help.instagram.com/833836199971426?helpref=uf_permalink) 兩個應用。

### 影子檔案

如果你不願意分享那么多數據，Facebook 會怎么做？它創建了[影子檔案](https://spideroak.com/articles/facebook-shadow-profiles-a-profile-of-you-that-you-never-created)或是「Facebook 收集的有關你沒有提供的數據集」。

正如這篇文章所述：

> 盡管你從未提供它們，但 Facebook 很有可能獲取了你的備用郵箱地址、電話號碼、家庭地址。所有這些都是由嘗試尋找并聯系你的朋友提供的。

更糟糕的是，Facebook 主要收集你的[面部](http://spectrum.ieee.org/biomedical/imaging/facebooks-face-recognition-tech-goes-on-trial)信息。

> 最近的一起訴訟不是針對郵箱地址和電話號碼，而是「人臉模板」：每當用戶上傳照片時，Facebook 會掃描所有人臉并創建「數字生物識別模板」。

即使 Facebook 只是為自己收集數據，所有這一切也是有關系的。但還有一些外部供應商。

## Facebook 和營銷人員是什么關系？

Facebook 的數據政策指出，它和其它供應商合作收集關於你的數據：

> 我們會從第三方合作伙伴收到有關你和你的 Facebook 在線與離線的活動信息。例如，當我們聯合提供服務時，來自合作伙伴的信息，或從廣告商那里獲得關於你的經曆、與他們互動的信息。

[Facebook 收集](http://www.techtimes.com/articles/190902/20161231/facebook-knows-a-lot-about-your-offline-habits-buying-third-party-data-to-serve-better-targeted-ads.htm)了「大約 29,000 個人口統計指標，其中 98% 基於用戶在 Facebook 的活動」。

> 與此同時，據報道大約有 600 個數據點來自 Experian，Acxiom等獨立數據代理商，用戶無法訪問從第三方獲得的人口統計數據。

除了收集你自願提供的所有詳細信息，比如姓名全稱、出生日期、興趣愛好、宗教信仰、以及所有你上過學和工作過的地方，Facebook 還會對它不知道的事情作出假設，這樣就可以與 Acxiom 、其它廣告代理商分享數據，以便更有效地把你作為目標。

比如，Facebook 使用家庭收入創建數據檔案賣給營銷商，他們畢竟是 Facebook 的付費客戶。然后，營銷人員可以購買細分資料，包括[以下任何一種](https://www.washingtonpost.com/news/the-intersect/wp/2016/08/19/98-personal-data-points-that-facebook-uses-to-target-ads-to-you/?noredirect=on&utm_term=.8f32259f05e5)：

地理位置、年齡、世代、性別、語言、教育水平、研究領域、學校、族裔關系、收入和淨資產、房屋所有權和類型、房屋價值、財產大小、房屋面積、建造年份、家庭組成。

Facebook 如何知道這些的？根據它所知道的和從 Experian 等處獲取的數據，[對你作出一些假設](https://www.quora.com/How-accurate-are-income-levels-in-Facebook-ad-targeting-and-how-does-Facebook-gather-this-information)。

這類數據隨后可以用來以廣告的形式定位 Facebook 用戶。在 Facebook 做的這種定位告訴你很多關於他們隱藏在幕后的數據。例如，不僅可以通過位置/年齡/性別/語言，還能通過興趣愛好和不同生活階段（如剛剛訂婚、6個月前訂婚、早期學齡兒童）定位目標。如此過細地定位一個人是有可能的，而且還能達到一定數量（在我的例子中是 100-200 人）。

![targeted.png](https://i.loli.net/2018/08/31/5b89330d1032f.png)

這些數據會被轉賣到下游，通過信用卡和其它營銷資源，與其它既存的關於你的數據混合在一起，從而創建類似[這樣的](http://www.familytreenow.com/)網站，試圖建立你的完整個人資料。沒有簡單的方式來擺脫它，因為一旦創建了數據，[刪除它難上加難了](http://idlewords.com/talks/haunted_by_data.htm)。這就是為什么隱私活動人士最關心的問題之一是讓公司每隔一段時間刪除大量數據。

Facebook 也有權在廣告里使用你和[未滿18歲孩子的照片](https://www.facebook.com/help/116356655118482?helpref=related)。

## Facebook 給政府提供什么數據？

我們并不了解 Facebook 提供給政府的所有信息。Facebook 有一個[政府報告頁面](https://govtrequests.facebook.com/)，該頁面自 2016 年6月以來沒有更新過。但我們知道政府還在要求獲取[越來越多的信息](https://techcrunch.com/2016/12/21/government-requests-for-facebook-user-data-up-27-percent-in-first-half-of-2016/)。

這些數據成為一份報告，報告顯示了數據訪問量和受影響的用戶量，但沒有提到任何關於所提供信息的類型、訪問數據的機搆類型（當地政府、州、聯邦調查局/國家安全局）。

| 國家   |  用戶數據要求總量  | 參考的用戶賬戶總數  | 產生某些數據請求的百分比   | 內容限制   | 保存要求   | 保留的用戶/帳號  |
|:----|:----|:----|:----|:----|:----|:----|
|  美國    |  23,854    |  38,951    |  80.65%    |  0    |  31893    |  56714    |

馬克·扎克伯格（Mark Zuckerberg）甚至發表聲明[說](https://www.facebook.com/zuck/posts/10100828955847631)：

> Facebook 過去不是，現在也從來沒有參與任何讓美國或任何其它政府直接訪問我們服務器的計划。我們從來沒有收到任何政府機搆的一般要求或法院命令，提供大量信息或元數據的，據說 Verizon 收到過這樣的要求。如果我們這樣做了，會積極與之抗爭。在昨天之前，我們甚至沒聽說過稜鏡計划。

在這里，重要的是從字里行間讀出的含義。直接訪問服務器不是發送大容量文件的必要條件，[也沒有必要以此名了解稜鏡計划](https://www.theguardian.com/world/2013/jun/06/us-tech-giants-nsa-data)。

也很難知道國家安全局是否[以其它方式從 Facebook](https://www.nytimes.com/2014/06/01/us/nsa-collecting-millions-of-faces-from-web-images.html) 收集數據。至少在歐洲，有關此問題的[訴訟正在進行中](http://fortune.com/2016/09/12/facebook-class-action-eu-privacy/)。

但就目前而言，僅僅假設這種[監控正在進行](http://www.cnn.com/2013/09/30/us/nsa-social-networks/)。

## 退出 Facebook 后，Facebook 會跟蹤什么？

在 Facebook 網站之外，Facebook 通過[單點登錄](http://venturebeat.com/2014/10/06/the-cookie-is-dead-heres-how-facebook-google-and-apple-are-tracking-you-now/)跟蹤用戶。

如果你退出，Facebook 也會通過 cookies 跟蹤你。正如它們的[隱私政策所述](https://www.macobserver.com/tmo/article/facebook-is-tracking-you-even-if-you-dont-have-an-account)：

> 當你訪問或使用第三方網站和應用了我們服務的程序時，我們會收集信息。收集的信息包括訪問的網站和應用程序、在這些網站和應用上使用我們的服務、以及網站或應用的開發者或發布者提供給你或我們的信息。

Facebook 也在試圖跟蹤或已經在跟蹤[你的光標在屏幕上的移動情況](http://blogs.wsj.com/cio/2013/10/30/facebook-considers-vast-increase-in-data-collection/)。

早在 2011 年，[如果你仍然登錄着 Facebook, 它就開始跟蹤你如何在網絡上移動](http://lifehacker.com/5843969/facebook-is-tracking-your-every-move-on-the-web-heres-how-to-stop-it)。

> 未經你同意，Facebook 會記錄你登錄后所在網頁的位置。Nik Cubrilovic 深入挖掘了一下，發現即使登出 Facebook 仍會跟蹤你的位置。Facebook 否定了這一說法。

可以肯定的是，Facebook [收集你的瀏覽曆史來丰富廣告。](http://gizmodo.com/how-to-stop-facebook-from-sharing-your-browsing-history-1589918083)

## 當我使用 Facebook 時應該考慮什么？

這一切意味着什么？從本質上講，它意味着你在 Facebook 上做的每件事情，或是通過其它網站登錄，都可能會被 Facebook 偷偷地跟蹤并保留在服務器上。

需要明確的是，很多公司目前都會對用戶進行某種形式的跟蹤。除此以外，沒有其它方式可以衡量經營活動。但是 Facebook 顯然在一段時間內躡手躡腳地走出了道德上可接受的數據業務實踐的范圍。盡管 Facebook 目前沒有做我提及的一些事情（抓取預發布內容、擾亂新聞訂閱源），但它們也在做着非常相似的工作，而且沒有隱私保障和，也不保證不用於實驗。這也意味着即使你在 Facebook 并不活躍，仍會被跟蹤。

每個像你這樣的人發的帖子、添加的每個好友、簽到的每個地方、點擊的每個產品類別、每張照片，都會保存在 Facebook 并被聚合在一起。

如何聚合？很難描述。可能是社會實驗的一部分，也許你的信息正被提交給政府部門；也許Facebook 的那些沒有必要擁有此權限的員工可以訪問你的頁面、查看你的工作經曆；也許相同的就業信息正被發送給保險公司。

這包括了所有的私人小組、封閉小組以及所有的消息。正如 Facebook 指出的，在 Facebook 不存在隱私這回事。

實質上，你需要加入 Facebook, 這意味着接受你做的每件事情都會被公開，或是被用於廣告、政府機搆分析。

## 如果不想讓 Facebook 獲取我的數據，應該怎么辦？

Facebook 開始是大學生互相聯系的一種方式，最終達到了改變人們行為、跟蹤用戶使用情況，并且可能為政府整合信息的程度。

問題在於無論誰是否使用 Facebook, 都牽涉到 Facebook 的跟蹤、關系標簽、影子檔案系統。如果你是 Facebook 活躍用戶，尤其如此。

因此，最重要的事情是意識到這種情況正在發生，并盡可能少給 Facebook 提供數據。

下列是我為了盡量減少在 Facebook 的曝光而做的事情。

并非每個人都會像我這樣做。但最重要的是，即使你決定繼續使用 Facebook , 也要知道Facebook 在使用你的數據做什么，并且有權在社交中作出權衡。

1. 不要發布過多的個人信息。
2. 不要發布你孩子的任何照片，特別是當他們處在無法同意的年齡。
3. 當你用瀏覽器訪問 Facebook 后, 退出 Facebook. 使用一個單獨的瀏覽器訪問 Facebook, 其它事情則用另一個單獨的瀏覽器。
4. 使用[廣告攔截](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=en)插件。
5. 組織或參與政治活動，不要使用 Facebook , 尤其是 Messenger 應用。如果你需要組織活動，用 Facebook 作為發起端，然后換用別的平台。推荐平台：Signal 是目前私密聊天的典范。Whatsapp 的群組聊天是可以的，但我不推荐它，因為它與 Facebook 的元數據系統緊密相聯。電報（Telegram）也不錯，但還不夠好，因為它不是開源應用。此外，它取決於你的風險等級。這是有關[這些平台](http://lifehacker.com/signal-the-encrypted-chat-app-is-now-available-on-des-1787103250)的[更多](https://www.relativisticramblings.com/ramblings/telegram-vs-signal/)信息。
6. 不要在手機上安裝 Facebook 應用程序，它會請求許多[不合理的權限](https://www.makeuseof.com/tag/use-facebook-android-without-invasive-permissions/)。
7. 不要在手機上安裝 Messenger 應用。使用移動端網站。目前，Messenger 應用在移動設備上被屏蔽，[可以在瀏覽器啟用桌面版](http://www.howtogeek.com/176932/how-to-disable-the-mobile-version-of-a-website-on-your-phone/)。

很遺憾，做得如此好的社交網絡在互聯網上也是最糟糕的。但是，在人們遠離這個平台或對它施加某種經濟壓力之前，任何都不會改變。

就我個人而言，作為一個數據專家，我個人所做的事情就是給發郵件給我的 Facebook 招聘人員發送以下信息：

親愛的招聘專員：

Facebook 收集、使用數據的方式，包括：

* 把用戶數據轉售給 Acxiom 這樣的廣告公司；
* [跟蹤用戶瀏覽情況](https://www.huffingtonpost.com/nate-hanson/how-to-stop-facebook-from_b_8160400.html)；
* [人臉識別](https://www.allbusiness.com/marketers-use-facebooks-facial-recognition-stalk-customers-2-11934-1.html)；
* 建立[影子檔案](https://www.dailydot.com/news/facebook-shadow-profiles-privacy-faq/)；
* 特別是社會科學實驗，比如[情感傳染\*](http://www.pnas.org/content/111/24/8788.full)；
* 新聞訂閱源中使用算法，創造[過濾器泡沫](http://Bursting the Facebook bubble: we asked voters on the left and right to swap feeds)；
* 最重要的一點，[Facebook 向國家安全局（NSA）等政府機搆提供獲取大量數據的訪問權限](https://venturebeat.com/2014/05/15/how-the-nsa-fbi-made-facebook-the-perfect-mass-surveillance-tool/)

這讓我不僅強烈反對在 Facebook 工作，而且使我有力地評估了自己使用 Facebook. 因為我從來不知道輸入這個系統的每個字符將如何被使用。

如果 Facebook 公司承諾要改變發展方向，并且

* 利用數據來解決這些問題
* 積極研究如何[刪除不必要的數據](http://idlewords.com/talks/haunted_by_data.htm)
* 積極研究非政府干預的私人安全通訊
* 并積極研究如何避免私人客戶數據被共享給不必要的第三方

我很想知道。

謹啟

Vicki

我們是社會性動物，我們想要連接、得到認可、分享、在其他人所在的平台上組織活動。目前而言，這是 Facebook 的優勢。此外，很難說 Facebook 完全是壞的：它的確把人們聯系起來，幫助組織聚會和活動，并且確實使世界更加互聯互通。

但是，作為 Facebook 用戶，我們和我們的數據是它的產品。而且，隨着我們對這些數據的使用方式了解更多，我們仍然可以按照它的規則使用 Facebook，但要對它有所了解。

[這里是黑客新聞討論區。](https://news.ycombinator.com/item?id=13559498)
