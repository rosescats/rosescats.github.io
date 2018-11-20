---
title: 密码安全｜《隐身的艺术》第一章摘要
top: 0
date: 2018-11-18
updated: 2018-11-20
tags: 隐私安全
categories: reading
---

![THe Art of the Invisibility: the world's most famous hacker teaches you how to be safe in the age of big brother and big data](https://i.loli.net/2018/11/18/5bf13d74df111.jpg)
<centerTHe Art of the Invisibility: the world's most famous hacker teaches you how to be safe in the age of big brother and big data</center>

延伸阅读文章：

- [How Develpers got Password Security so Wrong](https://blog.cloudflare.com/how-developers-got-password-security-so-wrong/?utm_source=wanqu.co&utm_campaign=Wanqu+Daily&utm_medium=website) / *by Junade Ali*

- [I've Just Launched "Pwned Passwords" V2 With Half a Billion Passwords for Download](https://www.troyhunt.com/ive-just-launched-pwned-passwords-version-2/#cloudflareprivacyandkanonymity) / *by Troy Hunt*

---

# 密码

我们使用密码存在的安全问题是：

- 密码字符过短；
- 相同密码在不同账户重复使用；
- 密码中含有账户名/个人真实属性信息。

对应的对策可以有：

- 增加密码字符长度。

- 使用密码管理器（例如 1Password、LastPass）给使用的每个网站设置随机、唯一的密码。

- 尽可能的启用双重身份验证（2FA），二次验证登录者身份。通常是通过手机短信、邮件、Authentication App 获取随机验证码。在网站 <https://turnon2fa.com> 可以查看到如何启用 2FA.

- 给密码管理器设置一个安全、容易记住的管理密码，并打开 2FA, 保存好备份代码。

- 复杂规则密码的更好替代方法是不使用已经被破坏泄漏的密码。

EPPB（Elcomsoft Phone Password Breaker）的目的是使执法机构、政府机构获取 iCloud 账户的软件，并且可以公开销售。

为了保护你的 iCloud 和其它在线账户，必须设置一个强密码。

除了工作相关的密码之外，还有那些可以保护大部分个人账户的密码。选择一个难以猜测出来的密码，并不能避免 oclHashcat 这类黑客工具可能攻破你的密码，但是它可以使破译过程变慢，使得攻击者转向更容易的目标。

我们可以合理猜想，在 2015 年 7 月的 Ashley Madison 黑客事件中，暴露出来的一些密码肯定正在被用于其它地方，包括银行账户、甚至工作电脑。在公布在网上的 110,000,00 个 Ashley Madison 密码中，最常见的是「123456」「12345」「password」「DEFAULT」「123456789」「qwerty」「12345678」「abc123」「1234567」。如果你看见你自己的密码有上述这些，你很可能容易受到数据破坏。

## Pwned 安全检查

### 邮箱账户

可以在网站 [https://www.haveibeenpwned.com](https://www.haveibeenpwned.com) 检查你的邮箱账户信息是否出现过泄漏。

![Selection_005](https://i.loli.net/2018/11/20/5bf41947679e3.png)

<center>邮箱账户没有发生过泄漏</center>

![Selection_007](https://i.loli.net/2018/11/20/5bf4195a38dc9.png)
<center>邮箱账户在 3 个网站发生过泄漏</center>

![Selection_008](https://i.loli.net/2018/11/20/5bf41a02b5fc7.png)
<center>邮箱账户发生泄漏的详细说明</center>

### 密码暴露

在 <https://haveibeenpwned.com/Passwords> 可以检查密码是否已经在数据泄漏中暴露，如果显示红色背景的以下信息，说明查询的密码已经不能再使用了。

![Selection_002](https://i.loli.net/2018/11/20/5bf4129e200a2.png)

如果显示结果是 Good news--no pwnage found!,也只是表示这个密码在密码泄漏库中没有，但并不表示它是强密码。

![Selection_003](https://i.loli.net/2018/11/20/5bf4155829958.png)

在延伸阅读《开发者如何错误地使用密码》文章中提到了 Troy Hunt, 他是澳大利亚微软区域总监兼微软开发者安全专家。从 2011 年开始参与微软社区里的网络安全问题。他参与的重要项目之一就是 [Have I been pwned](https://www.haveibeenpwned.com)，这是一项免费服务，收集了数据泄漏，帮助网民确认他们是否受到了网络恶意行为的影响。

在 21 世纪，我们可以做得更好，也就是用字母和数字组合的更长、更复杂的密码。以下是自动、手动两种作法。

## 自动管理密码：使用密码管理器

最简单的方式是放弃创建你自己的密码，使用简单的自动化生成。有若干数字密码管理工具。它们不仅可以把密码存储在一个加密的金库里，当你需要密码的时候也允许一键获取，密码管理工具还可以为每个网站生成新的强、独特的密码。

使用密码管理器会有两个问题。

- 其一，密码管理器使用一个管理员密码来获得其它密码。如果有人碰巧使用恶意软件感染了你的电脑，当恶意软件记录每次按键输入，会盗取密码数据和管理员密码。这下就完蛋了！黑客会利用密码管理软件的后门获取密码。
- 其二，如果你丢失了管理员密码，意味着你丢了所有密码。最终，即使你可以重置每个密码，但如果有大量账户，这将会是一个很大的工作量。

尽管存在这些缺点，但下列小技巧应该足够保证密码安全。

1. **强密码口令（短语），而不是密码，应该足够长，至少 20-25 字符。** 随机字符的作用最好，但人类大脑难以记住随机序列。所以需要使用一个密码管理工具。推荐使用开源的密码管理工具，只在你的电脑本地存储数据，例如 Password Safe、KeePass.

2. **对两个不同的帐号，从不使用相同的密码。** 密码管理工具可以生成和存储强而唯一的密码。

在延伸阅读中提到，从 20 世纪 70 年代开始考虑安全存储密码，经过了使用哈希处理、BCrypt 算法处理密码，算法处理已经来不及抵挡强制破解密码，再加上很多网站还没有限制连续重复登录请求、使用验证码的情况下，要求用户在设置密码的时候遵守「至少只用数字、标点符号」这类复杂规则，并**没有帮助解决密码重复使用、密码弱、将个人信息输入密码的问题**。

## 手动创建并写下密码

1. 用纸写下密码，不要直接把账户、密码全部写出来，例如：中国银行：3sto7ghendp1vbs*.
2. 用隐晦的词汇代替账户，密码只写一部分
## 密码保护之外的设备保护
不要轻易随便与别人共享帐号密码。

除了密码保护在线服务，也应该用密码保护个人设备（电脑、手机、平板等），需要设置一个开机密码或者屏保密码。 

### 三种常见的给手机（Android/iOS/其它类型）加锁方法

1. passcode：最常见的一种方式，以特别的顺序输入的一连串数字
    1. 不要用手机号码里的数字设置
    2. 有些设备也支持 text-based passcode , 字母与数字混合
2. 另一种是 visual
    Android：Android lock patterns：140704 种组合
    ![alps](https://i.loli.net/2018/11/18/5bf13c5e5a3c0.jpg)
3. 第三种：biometrics 指纹解锁，人脸识别

作者建议 Biometrics 和 passcode 结合使用。
