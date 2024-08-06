---
layout: post
title:  "Windows station test"
date:   2022-12-11 19:40:59 +0800
tags: 
---


Windows上访问Github一直会出现
>"OpenSSL SSL_read: Connection was reset, errno" 10054

或者

>"Failed to connect to github.com port 443 after 21146 ms: Timed out"

的错误，应该是GFW的屏蔽。

在网上找了一个很莫名其妙的解决方案，重置git的全局代理

`git config --global --unset https.proxy`
`git config --global --unset http.proxy`
