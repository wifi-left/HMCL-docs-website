# HMCL 多人联机常见问题

# 必读

- 本文将定时收集HMCL 多人联机常见问题与回答，若你在这里没有发现你想要的回答，欢迎前往[此视频](https://www.bilibili.com/video/BV1g3411Y7rC)下的评论区进行提问，我会定期前往回答，然后将问题上传至此，也欢迎加入[QQ群：212927890](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)进行问题讨论！

- 你可以使用`Ctrl+f`来方便查找你的答案

- **在阅读本文章前，请先确认 HMCL 版本是否为 <img src="https://img.shields.io/maven-central/v/org.glavo.hmcl/hmcl-stable?label=稳定版" style="zoom:130%;" /> 或 <img src="https://img.shields.io/maven-central/v/org.glavo.hmcl/hmcl-dev?label=开发版" style="zoom: 130%;" />，若不是，请在 [此处](https://zkitefly.github.io/hmclw/download.html)下载他。**
- 如果你想为此文档做贡献，你可以在 [Github]() 提交Pull requests。其中，图片要存放在仓库中的 Github 仓库中的 /assets/img/docs/multiplayer-faq 目录中放置图片

## 1 多人联机会话意外退出，退出码 2

### 问题

在使用多人联机时出现下面图片问题↓

![](/assets/img/docs/multiplayer-faq/1.png)

### 回答

如果你出现了这个问题，那说明你没有认真的阅读上面的[必读](#必读)！

**请先确认 HMCL 版本是否为  <img src="https://img.shields.io/maven-central/v/org.glavo.hmcl/hmcl-dev?label=开发版" style="zoom: 130%;" />，若不是，请在 [此处](https://zkitefly.github.io/hmclw/download.html)下载他。**

## 2 无法连接多人联机服务，你可以在多人联机页面的反馈中反馈问题

### 问题

在使用多人联机时出现下面图片问题↓

![]()

### 回答

由于你当前使用 HMCL 多人联机的人过多，鉴权服务器没有足够的资源来使用联机

你可以等待每个整点或半点，鉴权服务器会自动刷新一次

你可以询问[QQ群](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)中群主或管理员询问鉴权服务器是否正常工作

若你没有足够的耐心等待，你可以考虑使用凭证联机开启桥接服务（在[QQ群：212927890](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)中获得凭证）

## 3 加入房间失败，无法与对方建立链接

### 问题

在对方加入房间时出现下面图片问题↓

![]()

### 回答

请检查房主和你的HMCL版本是否一致

可尝试使用凭证开启桥接服务，普通的ptp无法联机，因为nat等级过差

请检查 HMCL检测出来的 NAT 类型不是 **极差或差** 环境 ，因为可能就是因为他而**无法进行联机**。在 **差** 环境下你能进入 NAT 类型为 **好** 环境的房间

## 4 安装失败，部分文件无法下载

### 问题

进入 HMCL 多人联机页面时出现下方图片问题↓

![]()

### 回答

请检查你的电脑是否能正常上网、关闭防火墙或杀毒软件以及添加 cato （HMCL多人联机核心）程序为白名单

## 5  找不到 cato 程序 

### 问题

在创建房间时发生如下图片问题↓

![]()

### 回答

请关闭 HMCL ，然后再次启动，此时你进入多人联机页面就会下载 cato （HMCL多人联机核心）程序了

## 6 创建联机房间失败，你的凭证可能无法正常工作，你可以使用空凭证再试

### 问题

使用凭证开启桥接模式，然后创建房间时发生下方图片问题↓

![]()

### 回答

请检查你的凭证是否填写错误

请询问你正在使用的凭证是否还在有效期内

请联系[QQ群](https://jq.qq.com/?_wv=1027&k=N4mHT9FD)中群主或管理员询问鉴权服务器是否正常工作，或者耐心等待十分钟。



