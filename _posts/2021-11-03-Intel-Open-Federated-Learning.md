---
layout: post
title: 'Intel OpenFL'
---

I started working on my PhD experiments. I am working on the new Intel Framework for Federated Learning: Intel OpenFL.

![_config.yml]({{ site.baseurl }}/images/openfl.png)

Link to <a href="https://github.com/intel/openfl">OpenFL</a>.
Open Federated Learning (OpenFL) is a Python 3 project developed by Intel Labs and Intel Internet of Things Group. It enables organizations to collaborately train a model without sharing sensitive information with each other.

There are basically two components in the library: the collaborator which uses local dataset to train a global model and the aggregator which receives model updates from collaborators and combines them to form the global model.

The aggregator is framework-agnostic, while the collaborator can use any deep learning frameworks, such as Tensorflow or PyTorch.

Just to take confidence with this new framework, I am trying something simple: understand if an architecture with only 1 collaborator is equal to a non federated case. I will use DNNs (in particular CNNs like VGG) on simple datasets like MNIST or CIFAR10.

UPDATE 12/11/2021: After more or less 7 days of experiments I think that the framework is not working well and that metrics in federated and nonn-federated scenarios are different. I wrote to an Intel developer of OpenFL and he confirmed that I am right: single collaborator metrics in federated and non-federated scenario are different even with fixed random seeds.
