---
layout: post
title: Extension of the benchmark, ITADATA22, IEEE TMI, Multi-Input NN in FL, Work for Cardiologists
---

Almost finished 1st year of PhD!

Here are some updates on my recent projects :)

The benchmark of Federated Learning on non-IID data, with title "Benchmarking FedAvg and FedCurv for Image Classification Tasks" has already been published to the conference ITADATA22, held in Milan in September 2022, 
so at the time of writing this post I have already presented the paper. Conference was at the Department of Computer Science in Milan. The conference was
at the first edition, so it was not a top conference. For this reason, we want to extend the project in order to submit to a high-ranked journal. The main
idea to extend the work is to add more results, like datasets and algorithms. However, I noted that changing normalization layer in most common neural networks
architectures give better results in terms of accuracy, wrt using Batch Normalization. Preliminary results show that Group Norm and Layer Norm give from 10 to 20% (more or less) more
of accuracy, in all the scenarios (uniform and non-iid). So, I am extending the benchmark considering the following factors:
- Datasets: CIFAR10, MNIST and MedMNIST.
- Classification model: ResNet-18
- Scenarios: Uniform, Quantity Skew, Labels, Pathological and Dirichlet Labels Skew, and Covariate Shift
- Normalization Layers: Batch Normalization, Group Normalization, Layer Normalization, Instance Normalization, Batch Renormalization, SYycBN (and maybe some else)
- Epochs per round: 1, 10, 30, 100
- Fairness of epochs (I fix epochs to 1000, and I change the number of rounds to obtain 1000 epochs): 1000 epochs by 1000 rounds, 500, 200, 100, 50, 20 and 10
- Number of Collaborators: 2,4,8,10
I hope that I will obtain good results, write good paper that will be accepted (maybe to IEEE Neural Networks and Learning Systems)

Then, the work made with PerCeIVe Lab had a major revision, so we are re-running experiments to satisfy the reviews, and then will be resubmitted.

With Walter Riviera, a PhD student working for Intel, we are working on two projects: FL using Intel SGX and Multi-Input Neural Networks in Federated Learning.
For the first project I will only help him, Iacopo and Gianluca to run experiments, while in the second one I will be the main worker. However, for SGX, the main idea
is the following: benchmark testing security on network (HTTPS), disk (Encryption) and memory (Trusted Execution Environments), on CV, NLP, Graph and classic ML tasks,
using OpenFL with Graphene (and maybe to create a jupyter workflow interface to automate the process). For the second project, the idea is to apply multi-input
neural networks in federated learning. This because lot of datasets (especially medical imaging datasets) are provided together with tabular datasets containing
additional information like sex, age, previous illnesses and so on, that can help the ML process.

Finally, I am working for another project of cardiologists: I have to impute a tabular dataset and then I have to apply a 3-way propensity score matching. I am
not so expert in this field, so I will do whatever they want, studying with practice!

Kiss kiss
