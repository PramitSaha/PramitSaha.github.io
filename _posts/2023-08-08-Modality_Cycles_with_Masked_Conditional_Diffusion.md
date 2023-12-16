---
layout: post
title:  "Modality cycles with masked conditional diffusion for unsupervised anomaly segmentation in MRI"
place: MMMI at MICCAI 2023
authors: Ziyun Liang, Harry Anthony, Felix Wagner & Konstantinos Kamnitsas
date:   2023-08-01 11:00:00 +0200
image: /images/masked_modality_cycle.png
categories: out-of-distribution-detection
paper: https://arxiv.org/abs/2308.16150
arxiv:
code: https://github.com/ZiyunLiang/MMCCD
poster: /docs/MICCAI_Conference_poster_Ziyun_Liang_2023.jpg
comments:
year: 2023 
---

<style>
@media (max-width: 768px) {
    .container {
        flex-direction: column;
        align-items: left;
    }
</style>


<div class="container" style="display: flex; align-items: center;">
    <div class="image" style="flex: 1; margin-right: 1cm;">
        <img src="/images/masked_modality_cycle.png" alt="Image" style="max-width:100%; height:auto;">
    </div>
    <div class="content" style="flex: 1;">
        <h2>Abstract</h2>
        <p>
The most challenging, yet practical, setting of semi-supervised federated learning (SSFL) is where a few clients have fully labeled data whereas the other clients have fully unlabeled data. This is particularly common in healthcare settings where collaborating partners (typically hospitals) may have images but not annotations. The bottleneck in this setting is the joint training of labeled and unlabeled clients as the objective function for each client varies based on the availability of labels. This paper investigates an alternative way for effective training with labeled and unlabeled clients in a federated setting. We propose a novel learning scheme specifically designed for SSFL which we call Isolated Federated Learning (IsoFed) that circumvents the problem by avoiding simple averaging of supervised and semi-supervised models together. In particular, our training approach consists of two parts - (a) isolated aggregation of labeled and unlabeled client models, and (b) local self-supervised pretraining of isolated global models in all clients. We evaluate our model performance on medical image datasets of four different modalities publicly available within the biomedical image classification benchmark MedMNIST. We further vary the proportion of labeled clients and the degree of heterogeneity to demonstrate the effectiveness of the proposed method under varied experimental settings.</p>
    </div>
</div>


The method is based on two fundamental ideas. First, we propose the use of cyclic modality translation as a mechanism for enabling abnormality detection. Image-translation models learn tissue-specific modality mappings, which are characteristic of tissue physiology. Thus, these learned mappings fail to translate tissues or image patterns that have never been encountered during training, and the error enables their segmentation. Furthermore, we combine image translation with a masked conditional diffusion model, which attempts to `imagine' what tissue exists under a masked area, further exposing unknown patterns as the generative model fails to recreate them. We evaluate our method on a proxy task by training on healthy-looking slices of BraTS2021 multi-modality MRIs and testing on slices with tumors. We show that our method compares favorably to previous unsupervised approaches based on image reconstruction and denoising with autoencoders and diffusion models.

Dive into our research!

<a href="https://arxiv.org/abs/2308.16150">&#x1F4C4; Paper</a> | <a href="/docs/MICCAI_Conference_poster_Ziyun_Liang_2023.jpg">&#x1F4CA; Poster</a> | <a href="https://github.com/ZiyunLiang/MMCCD">`</>` Code</a>
