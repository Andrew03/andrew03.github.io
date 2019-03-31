---
layout: post
title: TensorboardX with Google Colaboratory
subtitle: How to visualize losses in Tensorboard while using Google Colaboratory
tags: [google-colab, tensorboard]
comments: true
---

## Google Colaboratory
[Google Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb) is a 
service hosted by Google. It gives you a free, fairly powerful GPU for free! The only
downsides is that the VM connecting you to the GPU shuts down after 12 hours, so you
have to start up a new instance to get another 12 hours. You can however connect the VM to your
Google Drive and save and load data there to persist data across instances. The only
other major downside of this service is that its mainly for [Jupyter Notebooks](https://jupyter.org).

## Tensorboard
[Tensorboard](https://www.tensorflow.org/guide/summaries_and_tensorboard) is a package
that can be used to graph and visualize results while training neural networks. This is 
particularly useful for tracking results, since you can visualize losses dynamically
and track whether your model is learning, over-fitting, or under-fitting. This tutorial
uses [TensorboardX](https://github.com/lanpa/tensorboardX), which is Tensorboard for 
[PyTorch](https://pytorch.org/), the main deep learning framework I use.

![Plot](https://www.tensorflow.org/images/mnist_tensorboard.png)

## Using Both of Them
While its usually easy to use Tensorboard on a local machine, there's a bit of work you
have to do to set it up on Google Colaboratory. You also have to do some work to link 
your VM to your Google Drive, and write Tensorboard event files to your drive so they
persist across sessions. Below is a gist containing a minimalistic example of how to 
set up Google Colaboratory with Google Drive and TensorboardX.

{% gist 226c0329e5f9706e97c39714bcac9d91 %}
