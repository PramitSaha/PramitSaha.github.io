---
layout: post
title:  "Moves made easy: deep learning-based reduction of human motor control efforts leveraging categorical perceptual constraint"
place: Master's Thesis
authors: Pramit Saha
date:   2021-08-01 11:00:00 +0200
image: /images/model_isofed_2.png
categories: federated-learning
paper: https://open.library.ubc.ca/media/stream/pdf/24/1.0396540/3
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

The human speech motor control system takes advantage of the constraints in categorical speech perception space to reduce the index of difficulty of articulatory tasks. Taking this for inspiration, we introduce a perceptual mapping from speech-like complex multiple degree-of-freedom (DOF) movement of the hand to a controllable formant space, that allows us to leverage categorical perceptual constraints for reducing the difficulty level of hand motor control tasks. The perceptual network is modeled using long short term memory networks (LSTMs) aimed at optimizing a connectionist temporal classification (CTC) loss function. Our motor control mapping network consists of a graph convolutional neural network (GCNN) combined with LSTM encoder-decoder network, that is regularized with the help of the trained perception model. The mapping allows the user's hand to generate continuous kinematic trajectories at a reduced effort by altering the complexity of the task space. This is a human-in-the-loop system where the user plays the role of an expert assessor in evaluating the degree to which the network is capable of reducing the complexity of task space. Further, we quantitatively formulate the index of difficulty of the task space and the throughput of the user and demonstrate that our model is able to perform consistently well in generating trajectories with considerably reduced effort using mouse and data glove-based input devices.

Dive into our research!

<a href="https://open.library.ubc.ca/media/stream/pdf/24/1.0396540/3">&#x1F4C4; Paper</a> 
