---
title: about
layout: about
date: 2024-02-28 17:42:13
---

# 我是
常住深圳，广东韶关人。但是不会客家话^_^
平时在学习的过程中积累了一些笔记，遂搭建了这个网站进行分享和总结。

学网络七年，了解水晶头的制作、服务器开关机重启、网络/云原生/存储/安全等字的听写。
会写PC网页、移动端后台、微信小程序，有一些软件开发经验；平时也习惯性开发了 腾讯课堂自动签到+邮箱通知、逆向爬虫、ensp网络自动化平台、daphne-websocket聊天室等小项目。

平时除了写点好玩的小工具，空闲时间也爱玩玩Minecraft、Arknights、Apex，偶尔也会去游个泳。


# 关于网站
博客部署在阿里云服务器，采用Hexo&Fluid搭建，代码分离为了主仓库（代码仓库）、子仓库（文档仓库）放置在了Github。
后台采用Vue3&TypeScript-Vben框架完成前端部分开发，Python3-DjangoRestFramework框架完成后端部分开发，使用MySQL数据库存储。
笔记文件整体保存至Github作为子仓库，通过push触发文档子仓库的trigger，主仓库则以[webhook](https://docs.github.com/zh/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows#repository_dispatch)触发工作流，完成整体模块拉取和更新的指定部署工作流程。
整个项目遵循敏捷开发思路，基于Github、Gitlab实现代码托管、配置项管理 以及 CI/CD。

目前完成：
- 搭建博客与后台的GithubActions工作流与GitLab-Pipline，完成持续构建与部署
- 工作台接入阿里云OpenAPI、百度API、GithubAPI、和风天气API
- 后台文档管理、CI/CD管理、静态资源管理


## 后台系统

![后台PC工作台-阿里云OpenAPI、百度统计API、和风天气API接入](https://www.fishingrodd.cn/img/demo1.png)
![后台PC工作台 - 最近访问动态](https://www.fishingrodd.cn/img/demo2.png)

![移动端PC工作台](https://www.fishingrodd.cn/img/demo3.jpg)



## todo

目前整体应用还存在优化空间，挖坑待填：Celery异步文档IO任务