---
layout:     post
title:      "机器学习"
subtitle:   "机器学习的一些基础知识"
date:       2016-10-09
author:     "Fish"
header-img: "img/post-bg-markdown.jpg"
catalog:    true
tags:
    - 机器学习
    - 工作
---

> 最近有工作上的任务需要了解机器学习（以下简称ML），看再多遍也不如记下来

#机器学习的定义 Machine Learning definition

ML与任何领域都息息相关，高度跨学科，在计算机视觉、生物学、机器人和自然语言等领域都有作用；

ML源于对人工智能的研究，在最近被认为是计算机的新能力，很多无法编译的程序，可以通过学习型算法，让电脑自己学习，例如：手写识别，自动化飞行，医疗建设，亚马逊、淘宝的个性化推荐，甚至以后可能治愈癌症

Arthur Samuel(1959) Machine Learning:Field of study that gives computers the ability to learn without being explicitly programmed.

Tom Mitchell(1998) Well-posed Learning Problem:A computer program is said to learn from exprformancerience E with respect to some task T and some pee measure P,if its performance on T,as measured by P,improves with experience E.
**对于计算机程序来说，给它一个任务T和一个性能测量方法P，如果在经验E的影响下，P对T的测量结果得到了改进，那么就说该程序从E中学习**

## 监督学习 Supervised Learning

为算法提供数据，即一组“标准答案”，之后希望算法去学习标准输入和标准答案之间的联系，以尝试对我们的其他输入提供更标准的答案

根据结果可分为**回归问题**（需要预测的变量是连续的）和**分类问题**（离散而不连续）

多个输入变量和多个特征，当数据不能在有限维表示出来时————*支持向量机*的算法：把数据映射到无限维空间中

## 无监督学习 Unsupervised Learning

给数据，不给标准答案，然后寻找数据的结构

**聚类算法**

聚类算法可以进行图像处理，读取一张图片创建3D模型

应用：计算机集群组织、社会网络分析、市场划分、航天数据分析

**独立组件分析**

应用：文本处理、理解功能分级和机械数据比如电磁大脑，扫描的EEG数据

ICA算法：`[W,s,v] = svd((repmat(sum(x.*x,1),size(x,1),1).*x)*x');`
	
## 强化学习 Reinforcement Learning

不需要进行一次决策，在一段时间内做出一系列决策，需要找到一种方式来定义想要什么

应用：机器人领域、网页爬取

