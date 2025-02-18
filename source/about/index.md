---
title: about
layout: about
date: 2024-02-28 17:42:13
---

# 我是
会3D建模与压网线的Python攻城狮，常居深圳
平时在学习的过程中积累了一些笔记，遂搭建网站进行分享和总结。



# 关于网站
博客部署在阿里云服务器，采用Hexo&Fluid搭建，代码分离为了主仓库（代码仓库）、子仓库（文档仓库）放置在了Github。
后台系统采用私有部署的[onedev](https://onedev.io/)实现代码托管与CI/CD。~~（原先是使用GitLab进行托管和CI/CD的，但是由于沟槽的国区迁移要求，我选择弃用。）~~
后台采用Vue3&TypeScript-Vben框架完成前端部分开发，Python3-DjangoRestFramework框架完成后端部分开发，MySQL数据库存储，Nginx做代理转发。
同时基于Golang的net/http标准库实现了服务端的SSE应用，完成了工作流结束时的客户端http消息通知。
笔记文件整体保存至Github作为子仓库，通过push触发文档子仓库的trigger，主仓库则以[webhook](https://docs.github.com/zh/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows#repository_dispatch)触发工作流，完成整体模块拉取和更新的指定部署工作流程。
整个项目遵循敏捷开发思路，基于Github、Gitlab实现代码托管、配置项管理 以及 CI/CD。

![整体架构](https://www.fishingrodd.cn/img/architecture.png)

目前完成：
- 搭建博客与后台的Github CI工作流与GitLab Pipline，完成持续构建与部署
- 后台系统代码由GitLab迁移至onedev私有仓库并重新配置工作流
- 工作台接入阿里云OpenAPI、百度API、GithubAPI、和风天气API
- 后台文档管理、CI/CD管理、静态资源管理


## 后台系统
![后台PC工作台-阿里云OpenAPI、百度统计API、和风天气API接入](https://www.fishingrodd.cn/img/demo1.png)
![后台PC工作台 - 最近访问动态](https://www.fishingrodd.cn/img/demo2.png)
![后台PC工作台 - CICD管理](https://www.fishingrodd.cn/img/cicd.png)
![移动端PC工作台](https://www.fishingrodd.cn/img/demo3.jpg)


