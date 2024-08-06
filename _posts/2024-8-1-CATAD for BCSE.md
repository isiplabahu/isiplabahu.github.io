---
layout: post # 不用改变
title:  Demo for CATAD # 博客标题
date: 2024-8-1 12:11:00+0800 # 时间
description: Demo for "CATAD - Conformer-Based Adversarial Training with Adaptive Diffusion for Bone-Conducted Speech Enhancement" # 博客描述
tags: demo # 标签 -- 以空格分隔
categories: demo-posts # 分类 -- 不需要改变
related_publications: dzq2024 # 你的论文
featured: false # 是否在首页展示
thumbnail: # post 预览图, 可以留空, 如有需要请填写 /assets/xxx.jpg
---
## Enhancing Bone-Conducted Speech with CATAD( Conformer-Based Adversarial Training with Adaptive Diffusion)

- Due to the low-pass filtering effect of human tissues, the high frequency components of bone-conducted (BC) speech suffer severe attenuation, resulting in reduced speech quality and intelligibility. To address this issue, this paper proposes a novel adversarial learning network based on the Conformer architecture and an adaptive diffusion process. In the design of the generator, we deploy a TS-Conformer consisting of two Conformer modules that capture temporal and frequency dependencies, respectively, to enhance the expressiveness of speech features. To ensure the stability of the adversarial learning process and the diversity of the generated results, we adopt an adaptive diffusion process that adds noise to both generated and real data. This challenges the discriminator to distinguish between diffused real data and generated data. Experimental results on the ESMB dataset demonstrate that our proposed method significantly improves BC speech recovery, enhancing both speech
quality and intelligibility.

![model_arc](/assets/img/CATAD/Framework.png "demo")


| BC Speech                                                                                                                | AC Speech                                                                                                                | CATAD(ours)                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| <audio src="/assets/CATAD/enhanced_speech/bc_speech0_generated_e2e.wav" type="audio/wav" controls preload></audio>   | <audio src="/assets/CATAD/enhanced_speech/bc_speech0_generated_e2e.wav" type="audio/wav" controls preload></audio>   | <audio src="/assets/CATAD/enhanced_speech/bc_speech0_generated_e2e.wav" type="audio/wav" controls preload></audio>   |
| <audio src="/assets/CATAD/enhanced_speech/bc_speech302_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech302_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech302_generated_e2e.wav" type="audio/wav" controls preload></audio> |
| <audio src="/assets/CATAD/enhanced_speech/bc_speech310_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech310_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech310_generated_e2e.wav" type="audio/wav" controls preload></audio> |
| <audio src="/assets/CATAD/enhanced_speech/bc_speech311_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech311_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech311_generated_e2e.wav" type="audio/wav" controls preload></audio> |
| <audio src="/assets/CATAD/enhanced_speech/bc_speech328_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech328_generated_e2e.wav" type="audio/wav" controls preload></audio> | <audio src="/assets/CATAD/enhanced_speech/bc_speech328_generated_e2e.wav" type="audio/wav" controls preload></audio> |
