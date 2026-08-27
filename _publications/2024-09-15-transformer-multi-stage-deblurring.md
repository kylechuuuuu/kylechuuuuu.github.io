---
title: "基于Transformer的多阶段运动模糊图像修复网络"
collection: publications
permalink: /publication/2024-09-15-transformer-multi-stage-deblurring
excerpt: '提出一种基于Transformer的多阶段去模糊网络，采用高效Transformer模块、多分支前馈网络与多阶段残差处理，在GoPro数据集上PSNR达32.23 dB、SSIM达0.955，在HIDE数据集上PSNR达30.15 dB、SSIM达0.930。'
date: 2024-09-15
venue: '《计算机工程》(Computer Engineering), 2024, 50(9)'
paperurl: 'https://www.ecice06.com/CN/Y2024/V50/I9/276'
citation: '朱凯, 李理, 张彤, 江晟, 别一鸣. (2024). &quot;基于Transformer的多阶段运动模糊图像修复网络.&quot; <i>计算机工程</i>. 50(9): 276-285. DOI: 10.19678/j.issn.1000-3428.0068246'
---

运动模糊是导致图像退化的常见原因，其限制了图像的可读性和后续处理效果。针对卷积网络感受野有限以及常规多阶段网络中信息丢失的问题，本文提出一种基于Transformer的多阶段去模糊网络。网络采用多阶段编码器-解码器结构，在单个阶段内和多个阶段间采用跳跃连接来增强信息的传递：

- **高效Transformer模块**：采用通道注意力和深度卷积来处理图像的全局和局部信息
- **多分支前馈传播网络**：通过引入多个并行的分支，实现不同尺度和不同层次的特征提取和融合
- **多阶段残差处理**：实现更优的图像恢复结果

**实验结果**：在GoPro数据集上PSNR达到32.23 dB、SSIM达到0.955；在HIDE数据集上PSNR达到30.15 dB、SSIM达到0.930，优于DeepDeblur、DeblurGAN-V2等模型。

**关键词**：深度学习；Transformer模型；注意力机制；图像修复；多尺度网络

论文全文请见 [《计算机工程》官网](https://www.ecice06.com/CN/Y2024/V50/I9/276) 或 [DOI链接](https://doi.org/10.19678/j.issn.1000-3428.0068246)。
