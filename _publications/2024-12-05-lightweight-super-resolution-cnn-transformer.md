---
title: "Lightweight Single Image Super-Resolution Network Integrating CNN and Transformer"
collection: publications
permalink: /publication/2024-12-05-lightweight-super-resolution-cnn-transformer
excerpt: '提出交替 CNN-Transformer 模块（ACTB）与融合式 CNN 高效 Transformer（ICET），并设计多分支门控 CNN 与并行通道注意力两种新结构，在保持低模型复杂度的同时兼顾局部空间与全局通道信息；×4 放大下 Set5 达 32.32 dB、Manga109 达 30.78 dB PSNR，以更低计算量超越同量级轻量超分模型。'
date: 2024-12-05
link: 'https://doi.org/10.1007/978-3-031-78125-4_15'
venue: 'Pattern Recognition (ICPR 2024), LNCS vol. 15332, Springer, Cham, pp. 212-225'
paperurl: 'https://doi.org/10.1007/978-3-031-78125-4_15'
citation: 'Kai Zhu, Li Chen. (2024). &quot;Lightweight Single Image Super-Resolution Network Integrating CNN and Transformer.&quot; In: <i>Pattern Recognition. ICPR 2024. Lecture Notes in Computer Science</i>, vol 15332, pp. 212-225. Springer, Cham. DOI: 10.1007/978-3-031-78125-4_15'
---

基于 CNN 与 Transformer 的单图像超分辨率（SISR）方法近年来取得了显著进展，但现有方法往往堆叠大量网络层，导致性能要求与显存占用大幅上升，限制了模型的实际部署与可用性。为此本文提出：

- **ACTB（Alternating CNN Transformer Block）**：交替式 CNN-Transformer 模块，在 Transformer 模块内部与模块之间结合卷积以提升特征提取效率
- **ICET（Integrative CNN Efficient Transformer）**：融合式 CNN 高效 Transformer
- **Multi-branch Gated CNN**：多分支门控卷积，高效提取局部空间信息
- **Parallel Channel Attention**：并行通道注意力，高效提取全局通道信息

**实验结果**：在 ×4 放大因子下，模型在 Set5 上取得 **32.32 dB**、在 Manga109 上取得 **30.78 dB** 的 PSNR；与其它轻量化超分模型相比，以**更低的计算成本**取得更优性能，在保持高表现的同时维持了低模型复杂度。

**关键词**：SISR；CNN；Transformer；注意力机制；深度学习

**[🔗 论文全文（Springer，DOI）](https://doi.org/10.1007/978-3-031-78125-4_15)** ｜ 源代码：[github.com/kylechuuuuu/ICTSRN](https://github.com/kylechuuuuu/ICTSRN)
