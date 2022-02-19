---
title:  "排错指南"
date:   2021-10-09 23:18:02 +0800
categories: HMCL
toc: true
---

> 本文由 LIPiston 进行编写，wifi_left 进行修改

# 一些话
仅列出部分容易出现的报错，__如有其他典型日志可以提交至 [LIPiston@outlook.com](mailto:LIPiston@outlook.com)__

# 排错指南
首先你需要具备一定的判断能力  
其次你需要 __调 整 好 心 态__  
~~说不定待会解决完这个还会崩呢对吧~~

这个时候就有一个小难题 __你的英文怎么样__ 

## 原版 & Forge报错
### 内存不足
![1](./assets/img/docs/debug/vanilla_mem.png)

这个问题是十分好解决的也是最常见的  
我们需要根据崩溃原因来进行判断  
由此，我们可以将内存上调直到游戏正常运行或者流畅运行

## Fabric 报错
### 缺少前置
![2](./assets/img/docs/debug/fabric1.png)

在报错中，我们可以看到
在第二项中有这些 mod 需要部分组件
在第一项中 fabric 已经明确的给出了指南
按照指南我们只需要把 fabric 的组件补全即可
所以我们需要去下载前置 fabricapi

### 模组冲突
#### 一般情况
![3](./assets/img/docs/debug/fabric2.png)

我们现在发现有两个 mod 在报错
由第一项我们可以得知 optfabric 与 sodium 有冲突
所以选择性的去掉一项即可

#### 特殊情况
有些 mod 本来是兼容的，但是在预加载阶段显示不兼容。或者进行设置后可以启动游戏。
##### Optifabric + lithium
这俩玩意儿原本是可以一起加载的，但需要进行一些设置。
步骤：
1. 打开 mods 文件夹
2. 用压缩方式打开 lithium.jar，编辑 fabric.mod.json 文件：
   找到 `"breaks"`
   删除 `"optifabric": "*"` 并保存。（可以直接删除 breaks 项）
3. 同样方式打开 optifabric.jar，编辑 fabric.mod.json 文件：
   找到 `"breaks"`
   删除 `"lithium": "*"` 并保存。（可以直接删除 breaks 项）
4. 打开 config 文件夹（.minecraft/config)，编辑（若不存在请创建）lithium.properties 文件：
   `mixin.world.chunk_access=false`
   保存。然后就能启动游戏了。
