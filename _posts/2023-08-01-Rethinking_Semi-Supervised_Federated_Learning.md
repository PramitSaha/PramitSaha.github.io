---
layout: post
title:  "Rethinking Semi-Supervised Federated Learning: How to co-train fully-labeled and fully-unlabeled client imaging data"
place: MICCAI 2023
authors: Pramit Saha, Divyanshu Mishra, J. Alison Noble
date:   2023-08-01 11:00:00 +0200
image: /images/model_isofed_2.png
categories: federated-learning
paper: https://arxiv.org/abs/2310.18815
arxiv:
code: 
poster: 
comments:
year: 2023 
---

<style>
@media (max-width: 1000px) {
    .container {
        flex-direction: column;
        align-items: left;
    }
</style>


<div class="container" style="display: flex; align-items: center;">
    <div class="image" style="flex: 1; margin-right: 1cm;">
        <img src="/images/model_isofed_2.png" alt="Image" style="max-width:100%; height:auto;">
    </div>
</div>

**Abstract**

The most challenging, yet practical, setting of semi-supervised
federated learning (SSFL) is where a few clients have fully labeled data
whereas the other clients have fully unlabeled data. This is particularly
common in healthcare settings where collaborating partners (typically
hospitals) may have images but not annotations. The bottleneck in this
setting is the joint training of labeled and unlabeled clients as the objective function for each client varies based on the availability of labels.
This paper investigates an alternative way for effective training with labeled and unlabeled clients in a federated setting. We propose a novel
learning scheme specifically designed for SSFL which we call Isolated
Federated Learning (IsoFed) that circumvents the problem by avoiding simple averaging of supervised and semi-supervised models together.
In particular, our training approach consists of two parts - (a) isolated
aggregation of labeled and unlabeled client models, and (b) local selfsupervised pretraining of isolated global models in all clients. We evaluate our model performance on medical image datasets of four different
modalities publicly available within the biomedical image classification
benchmark MedMNIST. We further vary the proportion of labeled clients
and the degree of heterogeneity to demonstrate the effectiveness of the
proposed method under varied experimental settings

Dive into our research!

<a href="https://arxiv.org/abs/2310.18815">&#x1F4C4; Paper</a> 
