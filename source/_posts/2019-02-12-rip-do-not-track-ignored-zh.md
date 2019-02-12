---

title: 翻译：大家忽视了「不要跟踪」隐私标准

date: 2019-02-12

tags: 隐私安全

categories: translation

---

原文是[RIP "Do Not Track," the Privacy Standard Everyone Ignored](https://www.howtogeek.com/fyi/rip-do-not-track-the-privacy-standard-everyone-ignored/)

作者：[Chris Hoffman](https://twitter.com/chrisbhoffman)

「不跟踪」有一个崇高的目标：在每个浏览器中都有一个简单的选项，告诉网站不要跟踪你的浏览记录。原以为它的确做到了，但问题是：网站并不在乎这一点。

正如我们在2012年指出的那样，[「不跟踪」选项并不能阻止你被跟踪](https://www.howtogeek.com/126705/why-enabling-do-not-track-doesnt-stop-you-from-being-tracked/)。只要连接一个网站，它就会发送一条特殊的信息，要求网站不要跟踪。绝大多数网站忽略了这一点，从未真正改变。网站忽略请求不会得到惩罚，也没有理由尊重「不跟踪」的请求。

尽管如此，「不跟踪」已经拖了好几年。这个选项是 Google Chrome、Mozilla Firefox、Apple Safari、Microsoft Edge、Internet Explorer 浏览器的一部分。如果你因为在网上被跟踪而感到沮丧，那么可以勾选这个选项，可能会让你感觉好一点，但实际上这是误导，什么也没有做。

事实上，「不跟踪」已经被用来跟踪用户。如果你已经启用了「不跟踪」，那么关于你的额外信息就会被跟踪了。例如，广告商可以此投放与隐私相关的广告。

一段时间以来，每个人都满足于忽略这个毫无用处的选项，但现在看来 DNT 终于崩溃了。正如 [DuckDuckGo](https://spreadprivacy.com/do-not-track/) 提醒，苹果公司正从 Safari 浏览器[移除](https://developer.apple.com/documentation/safari_release_notes/safari_12_1_release_notes)「不跟踪」设置项。就像 [Gizmodo](https://gizmodo.com/apple-is-removing-do-not-track-from-safari-1832400768) 发现的那样，DNT 标准讨论工作在2019年1月17日悄然[结束](https://www.w3.org/TR/tracking-dnt/)。随着标准被放弃、第一个浏览器移除它，我们希望其它浏览器开发商也能追随苹果的脚步。

这样不好吗？不。「不跟踪」从没有消失，但被网站忽视。在这一点上，「不跟踪」选项起到了安慰剂的作用，仅仅通过显示「不跟踪」误导用户。去掉 DNT 已经是很久以前的事情了。

「不跟踪」的发展历史是混乱的。微软只是让问题变得更糟糕，2010年，IE10 默认启用了这个功能，导致更多网站忽略了它。这点特别有趣，因为[微软](https://privacy.microsoft.com/en-us/privacystatement/)从来就不遵守 DNT 设置，换言之「因为对于如何解释 DNT 还没有达成共识，微软服务目前没有对浏览器 DNT 作出反应。」

包含跟踪保护功能的当代浏览器不会等到业界达成「共识」之后才开始跟进。相反，他们主动屏蔽追踪器。苹果的 Safari 浏览器含有「[智能跟踪保护](https://www.howtogeek.com/327773/how-safaris-new-intelligent-tracking-prevention-works/)」，可以避免没有直接访问的网站跟踪用户。Mozilla Firefox 提供了一个[内容拦截功能](https://support.mozilla.org/en-US/kb/what-happened-tracking-protection)，可以拦截已知的跟踪器。

这并不是说跟踪或[定向广告](https://www.howtogeek.com/341487/how-to-opt-out-of-targeted-ads-around-the-web/)一定是坏事。有支持也有反对的理由。但是，作为一个团体，我们应该讨论它，而不是用一个误导性的选项分散注意力，因为它实际上什么都没有做。
