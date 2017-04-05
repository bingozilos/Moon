---
layout: post
title:  "Apache struts2 S2-045/S2-046 漏洞原理"
date:   2017-4-2
excerpt: "环境搭建、调试步骤及原理分析"
feature: http://i4.buimg.com/589989/8bc853f8a49c3b14.jpg
tags: [vulnerability analysis]
---

# Apache struts2 S2-045/S2-046 漏洞原理

## 0x01  漏洞介绍

#### 漏洞名称：
>Apache struts2  远程代码执行漏洞（S2-045/S2-046）

#### 漏洞编号：
>CVE-2017-5638

#### 发布时间：
>S2-045 2017-03-07
>S2-046 2017-03-22

#### 影响范围：
>Struts 2.3.5 – Struts 2.3.31
>Struts 2.5 – Struts 2.5.10

#### 漏洞描述：
>Apache Struts2使用基于Jakarta的上传机制，存在远程代码执行漏洞。可以通过构造Content-Type值（S2-046多一个触发点filename）进行触发漏洞，造成远程代码执行。

