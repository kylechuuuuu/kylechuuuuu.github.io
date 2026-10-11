---
title: "Fine-Grained Cerebrovascular Parsing in DSA via Structurally-Grounded Semantic Disentanglement"
collection: publications
permalink: /publication/2026-09-26-fine-grained-cerebrovascular-parsing-dsa
excerpt: '提出多编码器协同框架 AngioParse，面向 DSA 中的细粒度血管解析：双流编码器协同融合高召回全局二值先验与异源编码器的解剖级特征，自洽结构 grounding 机制约束各类别预测的并集落在血管支撑域内以提升连通性与拓扑有效性，解耦正交预测模块抑制特征混淆；在公开 DSA 数据集上取得 SOTA 分割性能，可准确区分六类血管。'
date: 2026-09-26
link: '/files/2026-miccai-angioparse-dsa.pdf'
venue: 'Medical Image Computing and Computer Assisted Intervention (MICCAI) 2026, LNCS vol. 16893, Springer, Cham, pp. 180-189'
paperurl: 'https://doi.org/10.1007/978-3-032-38236-8_18'
citation: 'Kai Zhu, Le Cao, Li Chen, Jun Cheng, Lei Mou, Yitian Zhao. (2026). &quot;Fine-Grained Cerebrovascular Parsing in DSA via Structurally-Grounded Semantic Disentanglement.&quot; <i>Medical Image Computing and Computer Assisted Intervention - MICCAI 2026</i>, LNCS vol. 16893, pp. 180-189. DOI: 10.1007/978-3-032-38236-8_18'
---

在数字减影血管造影（DSA）中，准确的脑血管定量评估与临床干预从根本上依赖于血管解析——即对血管树进行分割并加以区分标注。然而 DSA 固有的复杂血管拓扑、严重的血管重叠以及不一致的对比度增强带来了巨大挑战；因此现有工作大多局限于**二值血管分割**，忽略了精细临床分析所需的细粒度解剖分类。本文提出 **AngioParse**，一个专为细粒度血管解析设计的多编码器协同框架，通过三项关键机制保证解析精度：

- **双流编码器协同模块（Dual-stream Encoder Synergy）**：融合高召回的全局二值先验与来自异源编码器的细粒度解剖特征，提升定位精度
- **自洽结构 grounding 机制（Self-consistent Structural Grounding）**：以高召回二值血管先验正则化细粒度解析，约束各类别解剖预测的**并集落在血管支撑域之内**，从而改善连通性与拓扑有效性
- **解耦正交预测模块（Decoupled Orthogonal Prediction）**：将多目标学习拆分为并行分支以最小化特征混淆，增强类别判别力

**实验结果**：在公开 DSA 数据集上，AngioParse 不仅取得 **state-of-the-art** 分割性能，还展现出准确解析与区分 **六种**不同血管类别的优越能力。

**关键词**：DSA；Vascular Parsing；Multi-Encoder Fusion

**[📄 下载论文PDF](/files/2026-miccai-angioparse-dsa.pdf)** ｜ 论文全文也可见 [MICCAI Open Access](https://papers.miccai.org/miccai-2026/paper/3344_paper.pdf) 或 [DOI 链接](https://doi.org/10.1007/978-3-032-38236-8_18)。代码：[github.com/kylechuuuuu/AngioParse](https://github.com/kylechuuuuu/AngioParse)
