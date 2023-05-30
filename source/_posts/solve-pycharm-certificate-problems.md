---
title: 【解决】pycharm 打开项目时 "Server's certificate is not trusted" 弹窗问题
date: 2023-05-30 10:53:56
tags: "Idea 工具使用"
categories: "技术工具"
description: 解决 windows 下 pycharm 启动出现 `Server's certificate is not trusted` 提示框的问题
---


[![github](https://img.shields.io/badge/github-Terry-brightgreen.svg?style=social)](https://github.com/2218084076)
[![Terry-WeChat](https://img.shields.io/badge/WeChat-Terry📷-success.svg?style=flat)](https://raw.githubusercontent.com/2218084076/personal-blog/main/img/WeChat.jpg)
![Terry-Email](https://img.shields.io/badge/Email-17601306065@163.com-red.svg?style=flat)

> 解决 windows 下 pycharm 启动出现 `Server's certificate is not trusted` 提示框的问题

## 问题

在使用 pycharm 打开项目文件时，会出现一下提示框

<!--more-->

![Solve pycharm certificate problems](https://raw.githubusercontent.com/2218084076/personal-blog/main/source/image/d7278c9a.png)

## 解决

为了摆脱这种情况，我们需要让 Idea 自动接受不受信任的证书。

`Files` -> `Settings` -> `Tools` -> `Server Certificates` -> 勾选 `Accept non-trusted certificates automatically`

![8028820d.png](https://raw.githubusercontent.com/2218084076/personal-blog/main/source/image/8028820d.png)

此时，再打开 pycharm 就不会再弹出上述异常了

## 什么是服务器证书（Server's certificate）

服务器证书在建立安全通信时起着重要的作用。当客户端（例如浏览器）与服务器建立安全连接时，
服务器会向客户端发送其证书。客户端收到证书后，会验证证书的有效性，以确保正在连接的服务器是合法可信的。

当网站或应用程序处理您的数据的方式存在某些异常时，通常会触发 `不受信任的服务器证书` 错误。
当您的网络配置不正确时，通常会发生这种情况。

在当今居家办公越来越普遍的环境中，WiFi 或 VPN 连接也往往会导致此错误。
