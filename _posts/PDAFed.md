---
layout: post
title:  "Post-Deployment Adaptation with Access to Source Data via Federated Learning and Source-Target Remote Gradient Alignment"
place: MICCAI MLMI 2023
authors: Felix Wagner, Zeju Li, Pramit Saha, and Konstantinos Kamnitsas
date:   2023-08-02 10:00:00 +0200
image: /images/StarAlign.jpg
categories: federated-learning
paper:https://arxiv.org/pdf/2308.16735.pdf
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
        <img src="/images/StarAlign.jpg" alt="Image" style="max-width:100%; height:auto;">
    </div>
</div>

**Abstract**

Deployment of Deep Neural Networks in medical imaging is
hindered by distribution shift between training data and data processed
after deployment, causing performance degradation. Post-Deployment
Adaptation (PDA) addresses this by tailoring a pre-trained, deployed
model to the target data distribution using limited labelled or entirely
unlabelled target data, while assuming no access to source training data
as they cannot be deployed with the model due to privacy concerns
and their large size. This makes reliable adaptation challenging due
to limited learning signal. This paper challenges this assumption and
introduces FedPDA, a novel adaptation framework that brings the
utility of learning from remote data from Federated Learning into PDA.
FedPDA enables a deployed model to obtain information from source
data via remote gradient exchange, while aiming to optimize the model
specifically for the target domain. Tailored for FedPDA, we introduce a
novel optimization method StarAlign
(
Source-Target
Remote Gradient
Alignment) that aligns gradients between source-target domain pairs by
maximizing their inner product, to facilitate learning a target-specific
model. We demonstrate the method’s effectiveness using multi-center
databases for the tasks of cancer metastases detection and skin lesion
classification, where our method compares favourably to previous work.
Code is available at: https://github.com/FelixWag/StarAlign

Dive into our research!

<a href="https://arxiv.org/pdf/2308.16735">&#x1F4C4; Paper</a> 
