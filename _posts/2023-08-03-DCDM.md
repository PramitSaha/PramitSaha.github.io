---
layout: post
title:  "Dual Conditioned Diffusion Models for Out-Of-Distribution Detection: Application to Fetal Ultrasound Videos"
place: MICCAI 2023
authors: Divyanshu Mishra, He Zhao, Pramit Saha, Aris T. Papageorghiou, J.Alison Noble
date:   2023-08-02 11:00:00 +0200
image: /images/FLOWCHART_UPD.jpg
categories: federated-learning
paper: https://arxiv.org/pdf/2311.00469.pdf
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
        <img src="/images/FLOWCHART_UPD.jpg" alt="Image" style="max-width:100%; height:auto;">
    </div>
</div>

**Abstract**

Out-of-distribution (OOD) detection is essential to improve
the reliability of machine learning models by detecting samples that do
not belong to the training distribution. Detecting OOD samples effectively in certain tasks can pose a challenge because of the substantial
heterogeneity within the in-distribution (ID), and the high structural
similarity between ID and OOD classes. For instance, when detecting
heart views in fetal ultrasound videos there is a high structural similarity
between the heart and other anatomies such as the abdomen, and large
in-distribution variance as a heart has 5 distinct views and structural
variations within each view. To detect OOD samples in this context,
the resulting model should generalise to the intra-anatomy variations
while rejecting similar OOD samples. In this paper, we introduce dualconditioned diffusion models (DCDM) where we condition the model on
in-distribution class information and latent features of the input image
for reconstruction-based OOD detection. This constrains the generative
manifold of the model to generate images structurally and semantically
similar to those within the in-distribution. The proposed model outperforms reference methods with a 12% improvement in accuracy, 22%
higher precision, and an 8% better F1 score.

Dive into our research!

<a href="https://arxiv.org/pdf/2311.00469">&#x1F4C4; Paper</a> 
