---
layout: post
title: Paper accepted (VISAPP), meeting with Carlo Cavazzoni (Leonardo Company), correct work of OpenFL, creation of non-iid datasets and so on
---

I have not written for the last 15 days, so in the middle there has been a lot of work.

First of all, the paper "Transfer Learning via Test-Time Neural Networks Aggregation" has been accepted to the conference VISAPP. This paper is based on the work of my thesis. Authors are me, Alessio Chisari (new PhD at UniCT), Sebastiano Battiato (Lecturer in Computer Science at UniCT) and Valerio Giuffrida (Lecturer in Data Science at Edinburgh Napier University). I will be the presenter at the conference (first days of February), that will be held online. I am preparing a set of slides for the oral presentation (around 20 minutes).

Today I had a meeting with my supervisor Marco Aldinucci, and Carlo Cavazzoni, the Head of Computational R&D at Leonardo Company. The firm is interested in aspects of HPC and AI for predictive maintenance, video surveillance and so on. We decided that in order to get confidence with Federated Learning and with OpenFL, I will use the Intel framework with non-iid datasets and different architectures. The aim is to get a baseline that shows the behavior of different networks with different types of non-iidness, because, presumably, different networks will react in a different way to this problem.

Then, focusing on OpenFL, the developers uploaded a new version of the framework which contains also a jupyter notebook showing that fixing random seeds leads to the same result in both federated and non-federated cases. I ran the experiment on both CPU and CUDA, using the node1 of _lmancuso_ and I can confirm that it works. Here some values: non-federated case <a href="https://pastebin.com/MjD3eAB5">link</a> and OpenFL <a href="https://pastebin.com/KfuJCgjs">link</a>

Now, the problems of retrieving non-iid datasets fits well with another task that I was treating in these days. Roberto Esposito (assistant professor at UniTO) and Mirko Polato (researcher at UniTO) asked me to create a function that, taken whatever dataset (images or tabular datasets) returns one of the five non-iid settings (described in P. Kairouz et al., Advances and Open Problems in Federated Learning, 2009.) of the same dataset on which FL algorithms could be tested thoroughly. I implemented a simple function that can do this, and Mirko improved my work. The objectiva is to test their work, _Federated Adaboost_ using these datasets.

Tomorrow I will follow a two-days workshop on HPC and Quantum Computing by CINECA <a href="https://youtu.be/0I6lv8bL0WM">link</a>

I have also followed the European Pilot, an internation 4-years project on HPC and AI. <a href="https://eupilot.eu/">link</a>

_Stay tuned_
