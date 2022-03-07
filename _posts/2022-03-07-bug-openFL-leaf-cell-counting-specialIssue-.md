---
layout: post
title: Bug OpenFL, Cell/Leaf Counting, Special Issue FL Medical Imaging
---

Update 07-03-22 
Last update was exactly 1 month ago.
So, in these days I have encountered a weird bug on OpenFL. I had implemented an experiment of digits classification using MNIST, using different data splitters, in order to study non-iid cases.
I had implemented (correctly) the quantity skew, the random split and the dirichlet split. The idea is to set a benchmark using OpenFL, several NN architectures, different datasets and non-iid distributions.
However, thisi is the bug: basically, when running a long experiment (in terms of rounds of training) using 10 envoys there is (probably) a problem of critical race.
I have opened an issue on the github repository: <a href="https://github.com/intel/openfl/issues/356">link</a> It seems that the envoy tries to read the database before that someone writes it.
Moreover, about OpenFL, I created a video tutorial for YT, in which I show how to run a real federation using 2 different nodes, and using a jupyter notebook <a href="https://www.youtube.com/watch?v=jlX3kbDF5uY&t=333s">link</a>

About other projects: I am trying to work again with Prof. Valerio Giuffrida from Edimburgh in 2 different scenarios: cell counting and leaf counting. I am studying the code of a leaf segmentation project that we want to extend.

I am following EUPilot meetings, because with CINI and Leonardo we are involved, for a video inference problem (using YOLO). 

Finally, there is a special issue about Federated Learning in Medical Imaging in which I have the opportunity to work with the PerCeiVeLab (Prof. Spampinato) of Catania

Mad love, peace out
