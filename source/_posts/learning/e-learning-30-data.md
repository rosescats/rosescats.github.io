---

title: E-learning 3.0 核心概念之「数据」
date: 2018-10-27
updated: 2018-11-01
tags: el30
categories: learn

---

[第一节课](https://chenmei.xyz/post/learning-notes/e-learning-30)介绍了 web 1.0, web 2.0, web 3.0 的特点，也是不同阶段互联网技术发展的主流应用。

**这是 E-Learning 3.0 MOOC 第二节课程。从本节开始将依次讲解 Web 3.0 同时也是 E-Learning 3.0 涉及的 9 个核心概念。**

本节课程页面在[这里](https://el30.mooc.ca/cgi-bin/page.cgi?module=5)，Stehen Downes 和 [Shelly Blake-Plock](https://about.me/BlakePlock)（Yet Analytics 创始人）对谈：<https://www.youtube.com/watch?v=dsmdwnUwKkA>

---

这节课的信息量非常大，第一次听说 SCROM、xAPI、LMS、LRS 这些概念，需要从对数据演变过程和去中心化入手。

## 在线内容：从文件到数据

正如 Stephen Downes 在数据这节课的文章 <https://el30.mooc.ca/cgi-bin/page.cgi?post=68416> 里所说，web 1.0 时代基于客户端-服务器模式，以文件和网页为主，在线学习的内容呈现形式也是如此，它们之间没有很好的交互、呈现标准也会不统一，而且 DVD 这类资源存放在用户端，没办法不同多终端使用。web 2.0 出现了基于数据和平台互操作性的网络。web 3.0 时代则将平台作用削弱，直接是终端之间直接交互，也就是分布式网络，也就是 e-learning 3.0.

在这个过程中，我们对内容的理解从普遍的（现在依旧还在用的）word/pdf/excel/video 等形式文档，随着对内容交互、分布式、共享互相链接的增加，转变扩展到对关于内容、使用者（学习者）的更多**元数据**的获取和分析。

>  When we created a learning resource, we created data about that resource, and this contained fields like ‘title’ and ‘typical age range’. From there it is a very small step to putting our content into the database as well, and completely converting our document into data. Most web-based content today comes from some sort of database.

例如，创建一份在线数据表单来收集统计一些必要的信息。在这份表单制作中设置的字段和填表对象填写的信息都是数据。现在很多在线表单平台都会提供简单的数据统计分类。

再比如，Facebook、Google 都会收集有关用户的一切信息，作为分析的 metadata, 在文章[「使用 Facebook 时，应该考虑什么？」](https://chenmei.xyz/post/fan-yi/what-should-you-think-about-when-using-facebook)中，作者 Vicki Boykis 说明了 Facebook 获取用户数据之多，以及如何利用这些数据获利。

> The dependence on centralized sources for linked data has led to the rise of platforms like Facebook and Twitter, with the result that people no longer feel in control of their own data, and even worse, have difficulty accessing and sharing this data. Also, it has become increasingly difficult to read this data without being tracked and without being forced to view advertisements and unwelcome messages.

## 数据：从中心化到 去中心化

关键词：**去中心化**，**linked data**

如 Yet Analytics 创始人 Shelly Blake-Plock 所说「data goverance can be used for good or evil」(<https://www.lauraritchie.com/2018/10/25/el30-notes-week-1/>)。我们也可以看到、已经深刻体会到网络上个人隐私安全问题，即使在单纯的在线学习过程中，也需要考虑这一点。去中心化则是一种新的选择。

除了这一点，更重要的是因为众多数据资源需要直接被获取、便捷共享、互相链接、在不同终端随时随地使用，每个人都可以管理控制自己的数据。

在 web 2.0 时代，我们把来自不同来源的数据堆积放在同一个网页上，这些都是在网页平台的幕后操作的。浏览器仍然需要从单一的网页上收到内容来呈现和组合。如果我们可以直接获取源数据库，根据自己的需要来选择、组合数据。

> From the perspective of the browser, everything is pretty much the same. It doesn’t matter whether a web page was created from one data source or a dozen. The browser still had to visit a web page and still received content from that single source to assemble and display to the viewer.

web 3.0 是一个去中心化链接数据的时代。每个人都可以管理自己的数据，随时随地存储并使用。像 [Solid](https://solid.mit.edu/)、[IndieWeb](https://indieweb.org/) 项目就正在寻找方法，使用户可以创建和管理自己的数据。

## 学习者个人如何管理数据

Stephen Downes 与 Shelly Blake-Plock 对谈中谈到的用于记录、存储、分析学习进度的技术 SCORM、xAPI、LRS 等等，暂时还不想深入了解这些。昨天翻了中文圈的「[教育大数据国际联盟](http://xapi-cop.net/zh/)」网站，里面有一些关于 xAPI 的介绍。目前对我来说有些深奥，还用不到它们。

> Learning also becomes a process of being able to comprehend data, to be able to look at representations of data though dashboards and visualizations, and to be able to identify patterns and draw conclusions. It’s interactive, immersive and engaging, a process of learning how to perceive and comprehend rather than to decode and store. 

**学习也成为能够理解数据、通过仪表盘和可视化来观察数据表现，并能识别模式、得出结论。它是一个互动式、沉浸式、吸引人的过程，是一个学习如何感知（perceive）、理解（comprehend）的过程，而不是简单的解码和存储。**

作为一个自主学习者，在不想将这些数据交由互联网公司获取管理的情况下，个人如何管理自己的学习资源和进度？很高兴看到[「eLearning 3.0: How do I show my expertise?」](https://idstuff.blogspot.com/2018/10/elearning-30-how-do-i-show-my-expertise.html) 这篇思考文章。作者提出了很多问题，认为一个人记录更新自己的学习过程，取决于具体的情况（it depends）。
