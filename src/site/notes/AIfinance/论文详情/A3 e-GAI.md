---
{"dg-publish":true,"permalink":"/AIfinance/论文详情/A3 e-GAI/","dgPassFrontmatter":true}
---

《e-GAI: e-value-based Generalized α-Investing for  Online False Discovery Rate Control》
[ICML Poster e-GAI: e-value-based Generalized $\alpha$-Investing for Online False Discovery Rate Control](https://icml.cc/virtual/2025/poster/45378)

## 作者
任好洁-上海交通大学数学科学学院
[‪Haojie Ren‬ - ‪Google 学术搜索‬](https://scholar.google.com/citations?hl=zh-CN&user=qfd5nS8AAAAJ&view_op=list_works&sortby=pubdate)[上海交通大学工业工程与管理系](https://ieem.sjtu.edu.cn/szdy/3192.html)
邹长亮-南开大学统计与数据科学学院
[‪Changliang Zou‬ - ‪Google 学术搜索‬](https://scholar.google.com/citations?hl=zh-CN&user=LPwSdmwAAAAJ&view_op=list_works&sortby=pubdate)[统计与数据科学学院](https://my.nankai.edu.cn/stat/zzl/list.htm)

## 背景
在线多重假设检验

局限性：广义α-投资（GAI）算法仅在特定的依赖结构下能基于p-值实现在线错误发现率控制

e-LOND算法（Xu & Ramdas, 2024）利用e-值在任意依赖结构下实现在线FDR控制，但其检验效能显著不足，因为其检验水平来源于预定义的递减序列

## 方法
e-GAI框架能够在更一般的依赖条件下确保可证明的在线FDR控制，同时通过动态分配检验水平来提高检验效能

引入了在线错误发现比例的理想估计，并在条件有效性下确保在线错误发现率控制

e-GAI从风险规避的视角动态分配检验水平，这既依赖于先前的拒绝次数与历史成本，也为每次拒绝分配更少的α财富。

从风险规避的角度出发，为每次拒绝分配较少的α-财富

在线FDR控制程序——e-LORD和e-SAFFRON，并为长期性能提供了策略，以解决GAI框架中常见的“α枯竭”现象。

在复杂依赖下，e-LORD和e-SAFFRON均比e-LOND具有更高的检验效能。mem-e-LORD和mem-e-SAFFRON，以优化长期性能，缓解α枯竭问题。

e-GAI可推广至条件超均匀p-值，这使得e-GAI成为一个具有可靠理论保证和更高实用价值的通用性工具。

模拟和真实数据实验均证明了e-LORD和e-SAFFRON在FDR控制与检验效能方面的优势。

## **未来**

1.尽管e-SAFFRON提供了一种自适应的在线错误发现率控制程序，但如何更准确地估计原假设比例（如ADDIS算法（Tian & Ramdas, 2019）所做的那样）值得进一步研究。

2.如第3.1节所讨论，当了解更具体的依赖结构时，有望获得对FDP__e(t)更精确的估计。未来值得研究FDP__e(t)的分母与依赖结构之间的关系，以及在此类情况下如何设计更高效的检验水平分配策略。