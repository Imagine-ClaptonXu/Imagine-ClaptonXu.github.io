---
layout:     post
title:      uni-app 开发 记录
subtitle:   采过的坑
date:       2020-04-17
author:     Donbin
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - uni-app
---

### uni-app 打开 webview, 关闭 webview 的 navigationBarTitle(单独去除原生导航栏)

- App 平台同时支持本地网页，但本地网页及相关资源（js、css等文件）必须放在 uni-app 项目根目录->hybrid->html 文件夹下
- 引入 ```<web-view src=`/hybrid/html/${yourIndexHtml}.html`></web-view>```
- 配置关闭 webview 的 navigationBarTitle: pages.json 文件 pages 对应 webview 的路径下的 style 下增加 "navigationStyle": "custom"

> 参考: [uni-app导航栏开发指南](https://ask.dcloud.net.cn/article/34921)
<!-- ![](https://images.ifanr.cn/wp-content/uploads/2018/06/WWDC-21.jpg) -->
