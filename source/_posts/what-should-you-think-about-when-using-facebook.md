---

title: 使用 Facebook 时，应该考虑什么？
date: 2018-08-31 19:35
updated: 2018-11-02
tags: 隐私安全
categories: translation
top: 0

---

> 原文：[https://veekaybee.github.io/2017/02/01/facebook-is-collecting-this/](https://veekaybee.github.io/2017/02/01/facebook-is-collecting-this/)

![winnower.jpg](https://i.loli.net/2018/08/31/5b8931e1c585a.jpg)

<figcaption>Courbet, The Winnowers</figcaption>

摘要：Facebook 通过众多渠道使用数百种方法收集有关你的数据。你很难退出，但通过了解他们收集的内容，可以认识到 Facebook 平台的危险性，并选择以更严格的限制来使用 Facebook.

目录：
* [Facebook 如何收集数据](#Facebook如何收集数据)
* [在你发布之前，Facebook 知道什么](#在你发布之前，Facebook知道什么)
* [发帖之后：Facebook 收集有关你的内容](#发帖之后：Facebook收集有关你的内容)
* [Facebook 内部用你的数据做了什么](#Facebook内部用你的数据做了什么)
    * [影子档案](#影子档案)
* [Facebook 和 营销商是什么关系](#Facebook和营销商是什么关系)
* [Facebook 向政府提供哪些数据](#Facebook向政府提供哪些数据)
* [你退出 Facebook , Facebook 会跟踪什么](#退出Facebook后，Facebook会跟踪什么)
* [当我使用 Facebook 时，应该考虑什么？](#当我使用Facebook时，应该考虑什么？)
* [如果我不想让 Facebook 获取我的数据，应该怎样做？](#如果我不想让Facebook获取我的数据，应该怎样做？)

Facebook 无论好坏，已经成为我们的网络客厅、[第三空间](https://en.wikipedia.org/wiki/Third_place)。这是我们与好友交谈、发布新闻、组织活动、悼念逝者、庆祝婴儿出生、订婚、找新工作、展示新发型和假期的地方。

Facebook 平台已经占据了如此大的占有率，并且开始作为我们的[冥想盆](http://harrypotter.wikia.com/wiki/Pensieve)。因此，了解 Facebook 公司获取使用我们的希望、梦想、政治宣言、婴儿照片信息做什么尤为重要。

从获取数据开始。2014年，Facebook 工程师写到他们[每天可以获取大约 600TB 的数据](https://code.facebook.com/posts/229861827208629/scaling-the-facebook-data-warehouse-to-300-pb/)。

对比一下，《战争与和平》的文本大小是3.1MB；1966年的苏联版《战争与和平》电影时长7小时，大小是[8GB](https://www.reddit.com/r/iphone/comments/462isr/get_some_storage_back_by_trying_to_download_a/)。

因此，人们每天上传的数据总量相当于1.93亿本《战争与和平》书籍、75,000部《战争与和平》电影。

[Facebook 数据政策](https://www.facebook.com/policy.php) 概述了它收集的内容和如何处理数据。然而，和大多数公司一样，Facebook 忽视了实际要点，没有告诉用户到底发生会什么。

我揣测自己写每条状态更新时的按键，使我感到沮丧，对此决定做一些研究。以下所有信息来自科技商业新闻报导、学术出版物、我作为 Facebook 用户能够在客户端看到的内容。作为一名从事用户数据工作10年以上的专家，我在这篇文章中加入了自己的诠释。

如果任何一位 Facebook 员工想要对此篇文章进行纠正，我会很乐意听他们说并没有像下文所说的那样收集和处理用户数据。

## Facebook 如何收集数据

为了理解 Facebook 数据收集的工作原理，我绘制了一个（非常非常）简单的图表。用户将数据输入用户界面（应用程序），这是前端。

这些数据随后被收集到 Facebook 的数据库（这些数据库有很多），这是后台。

用户在前端看到的数据是后台数据的子集。

![facebookui.png](https://i.loli.net/2018/08/31/5b89330d60b19.png)

如果你对更多的技术规格感兴趣，Google 上面有很多架构图。Facebook 正处在处理大数据的前沿，它们的堆栈包括 Hive, Hadoop, HBase, BigPipe, MySQL, Memcached, Thrift 更多。所有这些都存放在许多大型数据中心，比如 Prineville Oregon 数据中心。

## 在发帖之前，Facebook 知道什么？

> 在点击"post"之前，Facebook 可能就开始收集数据了。当你编辑信息时，[Facebook 开始收集你的按键内容](http://www.slate.com/articles/technology/future_tense/2013/12/facebook_self_censorship_what_happens_to_the_posts_you_don_t_publish.html)。

Facebook [曾经使用这些数据来研究自我审查](http://www.aaai.org/ocs/index.php/ICWSM/ICWSM13/paper/viewFile/6093/6350)（研究报告 PDF）。

![prepost.png](https://i.loli.net/2018/08/31/5b89330ce3682.png)

研究员写道：

> 我们报告的结果来自一份探索性分析，检查 Facebook 「最后时刻」的自我审查，或者在写完后在 Facebook 被过滤的内容。我们在 17 天内收集了 390万名用户的数据，并将自我审查行为与用户描述、用户社交图表以及他们之间的互动特征联系起来。

这意味着，如果你发布了类似于「我只是讨厌我的老板，他把我逼疯了。」这样的内容。虽然在最后一刻删除了这句话，改写为「伙计，现在的工作真是太疯狂了」，Facebook 仍然知道你在删除之前输入的内容。

以下是他们用于研究的数据点：

![prethought.png](https://i.loli.net/2018/08/31/5b89330d1426a.png)

这里值得注意的是：就像不能确保未发布的内容不会被存储；用户删除帖子、评论和签到，不能确保数据真的被删除了。

因此，即使删除了帖子，Facebook 仍记录了它。Facebook 记录[元数据](http://www.ruanyifeng.com/blog/2007/03/metadata.html)，或记录有关你的数据的数据。比如，拨打电话的数据就是实际谈话内容，它的元数据是拨打电话的时间、地点和时长等信息。

对于 Facebook 来说，元数据和真实数据同等重要，它使用元数据推断你的身份。在 Chrome 浏览器使用开发者工具，可以相对容易地看到大量数据通过 xhr 从你的客户端传送到 Facebook 后端。我不是一个前端忍者（但实际上我很乐意和其中一位谈话，看看我们还能做些什么），但从一张图上，可以看到 Facebook 在追踪用户做某件事花费的时间吗？具体内容不确定，但它可能计算出了耗费在 Facebook 网站的时间。[Facebook 报道说](https://www.nytimes.com/2016/05/06/business/facebook-bends-the-rules-of-audience-engagement-to-its-advantage.html?_r=0)。

![xhr-fb.png](https://i.loli.net/2018/08/31/5b89330d36265.png)

顺便说一句，对于账户删除也是如此。

由于 Facebook 拥有如此多的系统和可以数据共混的地方，正如一位 Facebook 前顾问所写：

> 回答你提问的第一部分，「你可以付钱让 Facebook 彻底删除你的所有信息吗？」假设「彻底」意味着完全清除你留在 Facebook 的任何痕迹。答案是不会。

同样，如果删除帖子，并不能确保 Facebook 不会在后台数据库保存这个帖子，它只是不会显示在客户端页面。

只要你真的写了帖子、上传了图片，或是修改了任何信息，对于 Facebook 内部研究使用、转售给 Acxiom 这样的营销聚合商、[通过国家安全局这样的机构](http://www.nytimes.com/2013/09/29/us/nsa-examines-social-networks-of-us-citizens.html)和 NSA 的棱镜计划提供给美国政府，这一切都是绝对公平的游戏。

## 发帖之后：Facebook 收集关于你的什么数据

很显然，Facebook 收集你自愿提供给它们的所有数据：政治派别、工作地点、最喜欢的电影、最爱读的书、打卡签到的位置、评论、对帖子的任何所有反应。Facebook [允许你下载他们的数据库中关于你的数据子集](https://www.facebook.com/help/302796099745838)。

在我个人的数据子集中，我可以看到：

* 我上传的照片、标记了我的照片
* 视频
* 我曾经发布在自己时间线上的一切内容（包括我表示感兴趣的事情、人们发布在我的时间轴上的内容、共享的记忆）
* 好友、添加我为他们的好友
* 我的所有私人信息
* 我参加过的活动
* 我登录过的每一台设备

以及，我可能感兴趣的广告。这不是我自己写的东西，而是 Facebook 基于我发布的每条内容，利用算法生成的。

我们将会在广告部分讨论这个问题。

除了数据和元数据，Facebook 也跟踪用户的意图。上面已经探讨了其中一种跟踪方式：未发布的信息，另一种则是在视频中的[热图跟踪](https://techcrunch.com/2016/08/10/360-storytelling/)。

Facebook不仅知道关于你的一切信息，也了解你的朋友关系。一言以蔽之，Facebook 很了解你，尽管你没有完整填写你的个人资料、也没有主动发布到网站。

## Facebook 内部用你的数据做了什么？

Facebook 利用收集到的数据做了很多事情。

首先，Facebook 对信息进行简单查询用于提高网站性能或用于行业报告（例如，网站运行时间，[Facebook 用户数量](http://veekaybee.github.io/how-many-users-do-you-have/)，今天的广告收入是多少？）。这对于任何公司都是如此。

不过，对于 Facebook 来说有所转变。Facebook 有一个完整的工程团队致力于搭建工具，使得数据更易于用 SQL——类似基于 Hadoop 和 [Hive](https://www.facebook.com/notes/facebook-engineering/hive-a-petabyte-scale-data-warehouse-using-hadoop/89508453919/) 的语言——查询。尽管 Facebook 声称严格控制权限，有些用户却并[不这么认为](http://www.techtimes.com/articles/36186/20150227/who-access-account-details-facebook.htm#sthash.GXFknTxA.dpuf)。

> 唱片公司 Anjunabeats 主管 Paavo Siljamäki 在 Facebook 发帖提醒人们注意这个问题，访问该公司洛杉矶办事处时，可以很容易访问他的 Facebook 账户而无需他的密码。

这里是[ Facebook 员工访问私人数据的账户的更多说明](https://www.quora.com/Do-Mark-Zuckerberg-or-Facebook-employees-have-a-skeleton-key-granting-them-access-to-every-members-Facebook-profile-page-and-information)。

其次，Facebook 把用户作为实验对象进行学术研究。在数据政策中没有提到这一点，这很有意思， [Facebook Research 主页](https://research.fb.com/)的标题写着：「在 Facebook, 研究渗透到我们所做的一切。」

Facebook 有一个相当大的数据科学团队（[最新统计是 41 人](https://research.fb.com/people/page/3/?cat=6)）。我想说的是，一个拥有 15000 人同样规模的公司，如果它真的想要积极推动一个数据科学研究项目，可能只有 5 个数据科学家。

然而，直到 2014 年为止，还没有任何程序可以检查被访问的数据类型、以及进行怎样的研究。正如一位[前 Facebook 数据科学家写到](http://andrewledvina.com/code/2014/07/04/10-ways-facebook-is-the-devil.html)：

> 我在 Facebook 的时候，没有一个机构审查委员会来审查为内部目的进行实验的决定。一旦有人得出结论，他们决定要把这篇文章发表到杂志上，那么在可发表的内容上，确实存在反反复复的公共关系和法律问题。如果你想做一个实验，看看人们会点击绿色按钮还是蓝色按钮，你无需得到批准。同样，如果要测试新的广告定位系统，以查看用户是否点击了更多广告，是否收入增加，无需获得机构批准。

虽然他接着指出这在大多数以软件服务的公司中是正常的，但大多数 SaaS 公司在过去十多年中也没有精心收集人们生活中最私密的细节。

他继续说道：

> 大多数人在 Facebook 研究数据的基本目的是影响和改变人们的情绪和行为。他们一直在做这件事，让你更喜欢故事，点击更多的广告，花费更多时间在 Facebook 网站。

尽管这是大多数网站的目标，但每天[花费超过 40 分钟](http://www.businessinsider.com/how-much-time-people-spend-on-facebook-per-day-2015-7) 在企图在情感上削弱你的网站上，你可能需要三思而后行。

Facebook 除了挖掘文本内容、[研究我们的情绪](https://research.fb.com/support-when-you-re-feeling-blue/)，它还会[操纵它们](https://www.theguardian.com/technology/2014/jun/29/facebook-users-emotions-news-feeds)。

新闻 Feed 是操作的首选。特别是因为 Facebook 已经设计出尽可能吸引人的功能：它是我们神经系统的突触糖。Facebook 希望确保你[尽可能在 Feed ](http://newsroom.fb.com/news/2015/06/news-feed-fyi-taking-into-account-time-spent-on-stories/)多花时间，并为此花[更多时间来处理婴儿照片](https://www.wired.com/2014/04/babies-on-facebook/)和其它快乐的事情，以及那些引发争议和愤怒的新闻。而像「我今天吃过早餐」这样的正常状态不会引起任何反应。

这就是当今所谓过滤气泡是怎样兴起的。因为人们会点一些他们感兴趣的东西，所以 Facebook 就只呈现吸引用户的内容，这意味着其他观点、朋友和图片会从一个人的 Facebook Feed 中删除。如果想了解这种方式是如何工作的，可以参考 [Red Feed、Blue Feed](http://graphics.wsj.com/blue-feed-red-feed/), 展示了自由与保守的 Facebook Feed 的不同之处。

他们还在研究其它什么？首先是[同性恋出柜](gay)比例。Facebook 如何知道这些的？「在过去的一年里，大约有 80 万美国人更新他们的个人资料，表达同性吸引或专属性别」。

大量的 Facebook 研究都是关于图论，也就是我们和朋友间的关系图。换句话说，它正在对从未同意的学科进行人类学研究。

例如在近期，数据科学小组发表了一项关于[美国移民社区的社会关系](https://research.fb.com/publications/the-social-ties-of-immigrant-communities-in-the-united-states/)的研究。在报告中，研究员使用了以下数据：

> 我们将我们的分析限制在基于已经被确认的社交网络数据基础上的综合判断，这些人在分析前 30 天内至少使用过一次 Facebook. 我们使用个人资料中指定的家乡来确定用户的国籍。

> 此外，我们也把分析限制在目前至少有2个朋友居住在本国的人和目前居中在美国的另外 2 个朋友。我们的结果基于超过 1000 万满足这些标准的人的样本。整篇报告中，所有关于 Facebook 用户的引用都毋庸置疑地暗示了这些限制。

这些是我们知道的公开研究，他们还在做哪些非公开的研究？

Facebook 理所当然喜欢研究的另一个内容是[人脸](https://www.bloomberg.com/news/articles/2016-10-26/is-facebook-s-facial-scanning-technology-invading-your-privacy-rights)。每次你在照片中标记自己时，Facebook 会认出你，并且做相应调整。

> Facebook 鼓励用户在他们个人帖子中上传的照片中「标记」人，社交网络将收集到的信息储存起来。Facebook 使用一个叫作 DeepFace 的程序来匹配用户的其它照片。

![selfie.png](https://i.loli.net/2018/08/31/5b89330d3ab7e.png)

这个名为 DeepFace 的程序是获取更多准确标签的绝佳方式。它也是侵犯个人隐私的绝佳手段。比如，倘若你不想被标记该怎么办？假如你在政府抗议活动中？或者简单来说，如果你和一位朋友去听音乐会，不是和另一位朋友，却还不想让对方知道，该怎么办？

不幸的是，很快就没有隐私可言了。Facebook 正致力于[识别照片中人的身份](http://fortune.com/2015/06/23/facebook-facial-recognition/)。Facebook 上[关于 DeepFace 的论文](https://www.cs.toronto.edu/~ranzato/publications/taigman_cvpr14.pdf)指出，「人脸识别技术对社会和文化影响是深远的」，然而根本没有谈到人脸被标记的可能的隐私危险。[比如](http://spectrum.ieee.org/biomedical/imaging/facebooks-face-recognition-tech-goes-on-trial)：

 > 她说，『我们很快就会在商店里安装摄像头，以识别顾客的购物情况』。

他们怎么知道这些的？

因为这些数据是我们自愿提供的。每次更新状态、上传照片并做标记、给朋友发信息、在一个地方签到、登录 Facebook, 系统都会自动生成一条信息保存到数据库中——「嘿，这个人现在在Facebook 世界里。」，包括了 [Whatsapp](https://techcrunch.com/2016/08/25/whatsapp-to-share-user-data-with-facebook-for-ad-targeting-heres-how-to-opt-out/) 和 [Instagram](https://help.instagram.com/833836199971426?helpref=uf_permalink) 两个应用。

### 影子档案

如果你不愿意分享那么多数据，Facebook 会怎么做？它创建了[影子档案](https://spideroak.com/articles/facebook-shadow-profiles-a-profile-of-you-that-you-never-created)或是「Facebook 收集的有关你没有提供的数据集」。

正如这篇文章所述：

> 尽管你从未提供它们，但 Facebook 很有可能获取了你的备用邮箱地址、电话号码、家庭地址。所有这些都是由尝试寻找并联系你的朋友提供的。

更糟糕的是，Facebook 主要收集你的[面部](http://spectrum.ieee.org/biomedical/imaging/facebooks-face-recognition-tech-goes-on-trial)信息。

> 最近的一起诉讼不是针对邮箱地址和电话号码，而是「人脸模板」：每当用户上传照片时，Facebook 会扫描所有人脸并创建「数字生物识别模板」。

即使 Facebook 只是为自己收集数据，所有这一切也是有关系的。但还有一些外部供应商。

## Facebook 和营销人员是什么关系？

Facebook 的数据政策指出，它和其它供应商合作收集关于你的数据：

> 我们会从第三方合作伙伴收到有关你和你的 Facebook 在线与离线的活动信息。例如，当我们联合提供服务时，来自合作伙伴的信息，或从广告商那里获得关于你的经历、与他们互动的信息。

[Facebook 收集](http://www.techtimes.com/articles/190902/20161231/facebook-knows-a-lot-about-your-offline-habits-buying-third-party-data-to-serve-better-targeted-ads.htm)了「大约 29,000 个人口统计指标，其中 98% 基于用户在 Facebook 的活动」。

> 与此同时，据报道大约有 600 个数据点来自 Experian，Acxiom等独立数据代理商，用户无法访问从第三方获得的人口统计数据。

除了收集你自愿提供的所有详细信息，比如姓名全称、出生日期、兴趣爱好、宗教信仰、以及所有你上过学和工作过的地方，Facebook 还会对它不知道的事情作出假设，这样就可以与 Acxiom 、其它广告代理商分享数据，以便更有效地把你作为目标。

比如，Facebook 使用家庭收入创建数据档案卖给营销商，他们毕竟是 Facebook 的付费客户。然后，营销人员可以购买细分资料，包括[以下任何一种](https://www.washingtonpost.com/news/the-intersect/wp/2016/08/19/98-personal-data-points-that-facebook-uses-to-target-ads-to-you/?noredirect=on&utm_term=.8f32259f05e5)：

地理位置、年龄、世代、性别、语言、教育水平、研究领域、学校、族裔关系、收入和净资产、房屋所有权和类型、房屋价值、财产大小、房屋面积、建造年份、家庭组成。

Facebook 如何知道这些的？根据它所知道的和从 Experian 等处获取的数据，[对你作出一些假设](https://www.quora.com/How-accurate-are-income-levels-in-Facebook-ad-targeting-and-how-does-Facebook-gather-this-information)。

这类数据随后可以用来以广告的形式定位 Facebook 用户。在 Facebook 做的这种定位告诉你很多关于他们隐藏在幕后的数据。例如，不仅可以通过位置/年龄/性别/语言，还能通过兴趣爱好和不同生活阶段（如刚刚订婚、6个月前订婚、早期学龄儿童）定位目标。如此过细地定位一个人是有可能的，而且还能达到一定数量（在我的例子中是 100-200 人）。

![targeted.png](https://i.loli.net/2018/08/31/5b89330d1032f.png)

这些数据会被转卖到下游，通过信用卡和其它营销资源，与其它既存的关于你的数据混合在一起，从而创建类似[这样的](http://www.familytreenow.com/)网站，试图建立你的完整个人资料。没有简单的方式来摆脱它，因为一旦创建了数据，[删除它难上加难了](http://idlewords.com/talks/haunted_by_data.htm)。这就是为什么隐私活动人士最关心的问题之一是让公司每隔一段时间删除大量数据。

Facebook 也有权在广告里使用你和[未满18岁孩子的照片](https://www.facebook.com/help/116356655118482?helpref=related)。

## Facebook 给政府提供什么数据？

我们并不了解 Facebook 提供给政府的所有信息。Facebook 有一个[政府报告页面](https://govtrequests.facebook.com/)，该页面自 2016 年6月以来没有更新过。但我们知道政府还在要求获取[越来越多的信息](https://techcrunch.com/2016/12/21/government-requests-for-facebook-user-data-up-27-percent-in-first-half-of-2016/)。

这些数据成为一份报告，报告显示了数据访问量和受影响的用户量，但没有提到任何关于所提供信息的类型、访问数据的机构类型（当地政府、州、联邦调查局/国家安全局）。

| 国家   |  用户数据要求总量  | 参考的用户账户总数  | 产生某些数据请求的百分比   | 内容限制   | 保存要求   | 保留的用户/帐号  |
|:----|:----|:----|:----|:----|:----|:----|
|  美国    |  23,854    |  38,951    |  80.65%    |  0    |  31893    |  56714    |

马克·扎克伯格（Mark Zuckerberg）甚至发表声明[说](https://www.facebook.com/zuck/posts/10100828955847631)：

> Facebook 过去不是，现在也从来没有参与任何让美国或任何其它政府直接访问我们服务器的计划。我们从来没有收到任何政府机构的一般要求或法院命令，提供大量信息或元数据的，据说 Verizon 收到过这样的要求。如果我们这样做了，会积极与之抗争。在昨天之前，我们甚至没听说过棱镜计划。

在这里，重要的是从字里行间读出的含义。直接访问服务器不是发送大容量文件的必要条件，[也没有必要以此名了解棱镜计划](https://www.theguardian.com/world/2013/jun/06/us-tech-giants-nsa-data)。

也很难知道国家安全局是否[以其它方式从 Facebook](https://www.nytimes.com/2014/06/01/us/nsa-collecting-millions-of-faces-from-web-images.html) 收集数据。至少在欧洲，有关此问题的[诉讼正在进行中](http://fortune.com/2016/09/12/facebook-class-action-eu-privacy/)。

但就目前而言，仅仅假设这种[监控正在进行](http://www.cnn.com/2013/09/30/us/nsa-social-networks/)。

## 退出 Facebook 后，Facebook 会跟踪什么？

在 Facebook 网站之外，Facebook 通过[单点登录](http://venturebeat.com/2014/10/06/the-cookie-is-dead-heres-how-facebook-google-and-apple-are-tracking-you-now/)跟踪用户。

如果你退出，Facebook 也会通过 cookies 跟踪你。正如它们的[隐私政策所述](https://www.macobserver.com/tmo/article/facebook-is-tracking-you-even-if-you-dont-have-an-account)：

> 当你访问或使用第三方网站和应用了我们服务的程序时，我们会收集信息。收集的信息包括访问的网站和应用程序、在这些网站和应用上使用我们的服务、以及网站或应用的开发者或发布者提供给你或我们的信息。

Facebook 也在试图跟踪或已经在跟踪[你的光标在屏幕上的移动情况](http://blogs.wsj.com/cio/2013/10/30/facebook-considers-vast-increase-in-data-collection/)。

早在 2011 年，[如果你仍然登录着 Facebook, 它就开始跟踪你如何在网络上移动](http://lifehacker.com/5843969/facebook-is-tracking-your-every-move-on-the-web-heres-how-to-stop-it)。

> 未经你同意，Facebook 会记录你登录后所在网页的位置。Nik Cubrilovic 深入挖掘了一下，发现即使登出 Facebook 仍会跟踪你的位置。Facebook 否定了这一说法。

可以肯定的是，Facebook [收集你的浏览历史来丰富广告。](http://gizmodo.com/how-to-stop-facebook-from-sharing-your-browsing-history-1589918083)

## 当我使用 Facebook 时应该考虑什么？

这一切意味着什么？从本质上讲，它意味着你在 Facebook 上做的每件事情，或是通过其它网站登录，都可能会被 Facebook 偷偷地跟踪并保留在服务器上。

需要明确的是，很多公司目前都会对用户进行某种形式的跟踪。除此以外，没有其它方式可以衡量经营活动。但是 Facebook 显然在一段时间内蹑手蹑脚地走出了道德上可接受的数据业务实践的范围。尽管 Facebook 目前没有做我提及的一些事情（抓取预发布内容、扰乱新闻订阅源），但它们也在做着非常相似的工作，而且没有隐私保障和，也不保证不用于实验。这也意味着即使你在 Facebook 并不活跃，仍会被跟踪。

每个像你这样的人发的帖子、添加的每个好友、签到的每个地方、点击的每个产品类别、每张照片，都会保存在 Facebook 并被聚合在一起。

如何聚合？很难描述。可能是社会实验的一部分，也许你的信息正被提交给政府部门；也许Facebook 的那些没有必要拥有此权限的员工可以访问你的页面、查看你的工作经历；也许相同的就业信息正被发送给保险公司。

这包括了所有的私人小组、封闭小组以及所有的消息。正如 Facebook 指出的，在 Facebook 不存在隐私这回事。

实质上，你需要加入 Facebook, 这意味着接受你做的每件事情都会被公开，或是被用于广告、政府机构分析。

## 如果不想让 Facebook 获取我的数据，应该怎么办？

Facebook 开始是大学生互相联系的一种方式，最终达到了改变人们行为、跟踪用户使用情况，并且可能为政府整合信息的程度。

问题在于无论谁是否使用 Facebook, 都牵涉到 Facebook 的跟踪、关系标签、影子档案系统。如果你是 Facebook 活跃用户，尤其如此。

因此，最重要的事情是意识到这种情况正在发生，并尽可能少给 Facebook 提供数据。

下列是我为了尽量减少在 Facebook 的曝光而做的事情。

并非每个人都会像我这样做。但最重要的是，即使你决定继续使用 Facebook , 也要知道Facebook 在使用你的数据做什么，并且有权在社交中作出权衡。

1. 不要发布过多的个人信息。
2. 不要发布你孩子的任何照片，特别是当他们处在无法同意的年龄。
3. 当你用浏览器访问 Facebook 后, 退出 Facebook. 使用一个单独的浏览器访问 Facebook, 其它事情则用另一个单独的浏览器。
4. 使用[广告拦截](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=en)插件。
5. 组织或参与政治活动，不要使用 Facebook , 尤其是 Messenger 应用。如果你需要组织活动，用 Facebook 作为发起端，然后换用别的平台。推荐平台：Signal 是目前私密聊天的典范。Whatsapp 的群组聊天是可以的，但我不推荐它，因为它与 Facebook 的元数据系统紧密相联。电报（Telegram）也不错，但还不够好，因为它不是开源应用。此外，它取决于你的风险等级。这是有关[这些平台](http://lifehacker.com/signal-the-encrypted-chat-app-is-now-available-on-des-1787103250)的[更多](https://www.relativisticramblings.com/ramblings/telegram-vs-signal/)信息。
6. 不要在手机上安装 Facebook 应用程序，它会请求许多[不合理的权限](https://www.makeuseof.com/tag/use-facebook-android-without-invasive-permissions/)。
7. 不要在手机上安装 Messenger 应用。使用移动端网站。目前，Messenger 应用在移动设备上被屏蔽，[可以在浏览器启用桌面版](http://www.howtogeek.com/176932/how-to-disable-the-mobile-version-of-a-website-on-your-phone/)。

很遗憾，做得如此好的社交网络在互联网上也是最糟糕的。但是，在人们远离这个平台或对它施加某种经济压力之前，任何都不会改变。

就我个人而言，作为一个数据专家，我个人所做的事情就是给发邮件给我的 Facebook 招聘人员发送以下信息：

亲爱的招聘专员：

Facebook 收集、使用数据的方式，包括：

* 把用户数据转售给 Acxiom 这样的广告公司；
* [跟踪用户浏览情况](https://www.huffingtonpost.com/nate-hanson/how-to-stop-facebook-from_b_8160400.html)；
* [人脸识别](https://www.allbusiness.com/marketers-use-facebooks-facial-recognition-stalk-customers-2-11934-1.html)；
* 建立[影子档案](https://www.dailydot.com/news/facebook-shadow-profiles-privacy-faq/)；
* 特别是社会科学实验，比如[情感传染\*](http://www.pnas.org/content/111/24/8788.full)；
* 新闻订阅源中使用算法，创造[过滤器泡沫](http://Bursting the Facebook bubble: we asked voters on the left and right to swap feeds)；
* 最重要的一点，[Facebook 向国家安全局（NSA）等政府机构提供获取大量数据的访问权限](https://venturebeat.com/2014/05/15/how-the-nsa-fbi-made-facebook-the-perfect-mass-surveillance-tool/)

这让我不仅强烈反对在 Facebook 工作，而且使我有力地评估了自己使用 Facebook. 因为我从来不知道输入这个系统的每个字符将如何被使用。

如果 Facebook 公司承诺要改变发展方向，并且

* 利用数据来解决这些问题
* 积极研究如何[删除不必要的数据](http://idlewords.com/talks/haunted_by_data.htm)
* 积极研究非政府干预的私人安全通讯
* 并积极研究如何避免私人客户数据被共享给不必要的第三方

我很想知道。

谨启

Vicki

我们是社会性动物，我们想要连接、得到认可、分享、在其他人所在的平台上组织活动。目前而言，这是 Facebook 的优势。此外，很难说 Facebook 完全是坏的：它的确把人们联系起来，帮助组织聚会和活动，并且确实使世界更加互联互通。

但是，作为 Facebook 用户，我们和我们的数据是它的产品。而且，随着我们对这些数据的使用方式了解更多，我们仍然可以按照它的规则使用 Facebook，但要对它有所了解。

[这里是黑客新闻讨论区。](https://news.ycombinator.com/item?id=13559498)
