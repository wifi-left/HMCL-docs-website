# HMCL 多人联机常见问题

# **必读**

- 本文将定时收集HMCL 多人联机常见问题与回答，若你在这里没有发现你想要的回答，欢迎前往[此视频](https://www.bilibili.com/video/BV1g3411Y7rC)下的评论区进行提问，我会定期前往回答，然后将问题上传至此，也欢迎加入[QQ群：212927890](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)进行问题讨论！

- 你可以使用`Ctrl+f`来方便查找你的答案

- **在阅读本文章前，请先确认 HMCL 版本是否为 <img src="https://img.shields.io/maven-central/v/org.glavo.hmcl/hmcl-dev?label=开发版" style="zoom: 130%;" />，若不是，请在 [此处](https://zkitefly.github.io/hmclw/download.html)下载他。**
- 如果你想为此文档做贡献，你可以在 [Github]() 提交 Pull requests 。其中，图片要存放在 Github 仓库中的 `/assets/img/docs/multiplayer-faq` 目录中

## **1 多人联机会话意外退出，退出码 2**

### 问题

在使用多人联机时出现下面图片问题↓

![](/assets/img/docs/multiplayer-faq/1.png)

### 回答

**请确认 HMCL 版本是否为  <img src="https://img.shields.io/maven-central/v/org.glavo.hmcl/hmcl-dev?label=开发版" style="zoom: 130%;" />，若不是，请在 [此处](https://zkitefly.github.io/hmclw/download.html)下载他。**

## **2 无法连接多人联机服务，你可以在多人联机页面的反馈中反馈问题**

### 问题

在使用多人联机时出现下面图片问题↓

![](/assets/img/docs/multiplayer-faq/2.png)

### 回答

**由于你当前使用 HMCL 多人联机的人数过多，鉴权服务器没有足够的资源来使用联机**

**你可以尝试等待每个整点或半点，鉴权服务器会自动刷新一次**

**你可以尝试询问[QQ群：212927890](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)中的群主或管理员鉴权服务器是否正常工作**

**若你没有足够的耐心等待，你可以考虑申请凭证开启桥接服务（询问[QQ群：212927890](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)中的群主或管理员获得凭证）**

## **3 加入房间失败，无法与对方建立链接**

### 问题

在对方加入房间时出现下面图片问题↓

![](/assets/img/docs/multiplayer-faq/3.jpg)

### 回答

**请检查房主和你的HMCL版本是否一致**

**可尝试使用凭证开启桥接服务，普通的 ptp 无法联机，因为这样的 NAT 类型会为 差或极差** 

**请检查 HMCL检测出来的 NAT 类型不是 差或极差 ，因为可能就是因为他而无法进行联机。在 NAT 类型为 差 下你能进入 NAT 类型为 好 的房间**

## **4 安装失败，部分文件无法下载**

### 问题

进入 HMCL 多人联机页面时出现下方图片问题↓

![](/assets/img/docs/multiplayer-faq/4.png)

### 回答

**请确认 HMCL 版本是否为 <img src="https://img.shields.io/maven-central/v/org.glavo.hmcl/hmcl-dev?label=开发版" style="zoom: 130%;" />，若不是，请在 [此处](https://zkitefly.github.io/hmclw/download.html)下载他**

**请检查你的电脑是否能正常上网、关闭防火墙、关闭杀毒软件或添加 cato （HMCL多人联机核心）程序为白名单**

**（一般这种问题应该是下载 cato 的服务器出现了一些问题，这种问题应该不会持续太久）**

## **5  找不到 cato 程序**

### 问题

在创建房间时发生如下图片问题↓

![](/assets/img/docs/multiplayer-faq/5.png)

### 回答

**请关闭 HMCL ，然后再次启动，此时你进入多人联机页面就会下载 cato （HMCL多人联机核心）程序了**

## **6 创建联机房间失败，你的凭证可能无法正常工作，你可以使用空凭证再试**

### 问题

使用凭证开启桥接服务，然后创建房间时发生下方图片问题↓

![](/assets/img/docs/multiplayer-faq/6.png)

### 回答

**请检查你的凭证是否填写错误**

**请检查你正在使用的凭证是否处于有效期内**

**请询问[QQ群：212927890](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)中的群主或管理员鉴权服务器是否正常工作，或者耐心等待十分钟。**

## 7 **无法检测游戏端口号，你必须先启动游戏并在游戏内打开对局域网开放选项后才能启动联机**

### 问题

创建房间时检测不到游戏端口，上面的小横条一直在动，如图↓

![](/assets/img/docs/multiplayer-faq/7.png)

![](/assets/img/docs/multiplayer-faq/8.png)

### 回答

*目前我们并不知道具体有效的修复方法（如果你知道，欢迎提交 Pull requests 来完善本文章，或者加入[QQ群：212927890](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)与我们进行讨论）*

**请检查是否开启游戏中的 对局域网开放 选项**

**你可以尝试重启一下电脑？**

**你可以尝试重新安装你的 JRE 或 JDK ，或使用不同的 JRE 或 JDK 来启动 HMCL 和游戏（建议安装[Liberica JDK](https://bell-sw.com/pages/downloads/)）**

## 8 **是否允许使用离线账号的玩家创建或加入房间**

### 问题

因为我和我的朋友没有正版账号与外置登录账号（authlib-injector），所以使用离线账号来进行创建或加入房间，是否允许？

### 回答

**允许，你和你的朋友可以使用离线账号来进行创建或加入房间**

**房主允许使用离线账号、正版账号和外置登录账号（authlib-injector）进行创建房间操作**

**加入方允许使用离线账号、正版账号和外置登录账号（authlib-injector）进行加入房间操作**

**注：加入方若使用离线账号，那么必须点击如在下方图片↓显示的 HMCL 多人联机房间按钮进入！否则无法进入**

![](/assets/img/docs/multiplayer-faq/9.jpg)

## 9 **X**

### 问题

X

![]()

### 回答

**X**
