---
title: M1 Mac安装Rosetta 2
date: 2021-08-28
author: 夏明
---

如何在M1 Mac上运行x86应用？新购买的M1 Mac，比如M1 MacBook Pro等机子上，如果想要运行x86应用，则需要Rosetta 2技术。但是有些M1 Mac上却并未安装Rosetta 2，因此需要自己手动安装Rosetta 2，该如何操作呢？

## 第一种方法

如果您在M1 Mac上有任何可用的x86应用，只需启动该应用就会提示用户安装Rosetta 2。单击“安装”，然后就可以将Rosetta 2安装到M1 Mac上了。

## 第二种方法

在Mac上安装Rosetta 2的另一种方法是使用熟悉的`softwareupdate`命令行工具。

```
softwareupdate --install-rosetta
```

这将启动rosetta 2安装程序，您必须同意许可协议，您会在每次在每台设备上安装任何东西时都做完整而透彻的阅读。

您还可以通过提供其他标志来跳过许可协议：

```
/usr/sbin/softwareupdate --install-rosetta --agree-to-license
```
