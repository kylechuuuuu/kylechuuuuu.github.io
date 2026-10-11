---
title: "Dual-level Adapter Boosting Prompt-free Curvilinear Structure Segmentation"
collection: publications
permalink: /publication/2026-06-01-dual-level-adapter-curvilinear-segmentation
excerpt: '提出通用曲线结构分割框架 SACM：在预训练 SAM 之上引入双层适配器（块内 internal adapter 细化细薄曲线局部表征 + 跨块 external adapter 做全局多层上下文聚合与域对齐），配合多层特征 FFN 融合与掩码解码器双阶段细化，仅用 18 张标注图像微调即在 12 个曲线数据集上实现 SOTA，无需提示（prompt-free）。'
date: 2026-06-01
link: '/files/2026-cvpr-sacm-curvilinear-segmentation.pdf'
venue: 'IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2026, pp. 36300-36310'
paperurl: 'https://openaccess.thecvf.com/content/CVPR2026/html/Zhu_Dual-level_Adapter_Boosting_Prompt-free_Curvilinear_Structure_Segmentation_CVPR_2026_paper.html'
citation: 'Kai Zhu, Li Chen, Jun Cheng. (2026). &quot;Dual-level Adapter Boosting Prompt-free Curvilinear Structure Segmentation.&quot; <i>Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)</i>, pp. 36300-36310.'
---

曲线结构分割在医学影像、遥感、材料科学等领域都至关重要，但现有方法往往需要大量领域内训练，且难以泛化到新领域。本文提出 **SACM（Segment Anything Curve Model）**——一个建立在预训练 **SAM** 之上的通用曲线分割框架，通过双层适配器同时实现细粒度增强与领域自适应：

- **Internal Adapter（块级）**：嵌入每个 Transformer block 内部，在局部适配并细化细薄、复杂的曲线结构表征
- **External Adapter（跨块）**：跨 block 捕获全局、多层上下文信息，完成跨域特征对齐与领域自适应
- **多层特征融合**：聚合所有 external adapter 的多层特征，经 FFN 模块融合
- **双阶段掩码解码细化**：在 mask decoder 中增强拓扑结构与连通性

该设计支持 **prompt-free、数据高效的微调**：仅用 **18 张标注图像**训练即可获得稳健的跨域泛化能力，并在 **12 个**多样化曲线结构数据集上取得 **state-of-the-art** 性能。

**[📄 下载论文PDF](/files/2026-cvpr-sacm-curvilinear-segmentation.pdf)** ｜ 论文全文也可见 [CVF Open Access](https://openaccess.thecvf.com/content/CVPR2026/html/Zhu_Dual-level_Adapter_Boosting_Prompt-free_Curvilinear_Structure_Segmentation_CVPR_2026_paper.html) 或 [OpenReview](https://openreview.net/forum?id=Z5WdKBoMMJ)。
