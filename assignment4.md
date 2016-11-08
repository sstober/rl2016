---
layout: default
title: Assignment 4
id: ass4
---


# Assignments 4: CNNs

In these assignments, we will will continue to explore common neural network designs and extend our focus towards convolutional neural networks a.k.a. CNNs or convnets. 

## Basic Reading

Please start by reading the full [Deep Learning Book - Chapter 9: Convolutional Networks](http://www.deeplearningbook.org/contents/convnets.html). Sections 9.10 and 9.11 are optional. This should give you a good overview of this domain and forms a common basis for everybody.

Post your remarks, insights and open questions in your blog and in the forum! Help each other to make sure you are not getting stuck too long with some unresolved issue.

**Deadline for questions to be considered in class is November 12, 7am**. 
I will also try to accommodate things that come in later but I cannot make guarantees. The earlier you bring up questions, the better.


## Further Reading

### Dilated Convolution

Read these papers with focus on the dilated convolution technique!

* Yu & Koltun [Multi-Scale Context Aggregation by Dilated Convolutions](https://arxiv.org/abs/1511.07122)
* [The Deepmind blog post on "WaveNet: A Generative Model for Raw Audio"](https://deepmind.com/blog/wavenet-generative-model-raw-audio/) has a nice animation of how dilated convolution works. There is also a [paper](https://arxiv.org/abs/1609.03499).

### CNNs for Speech Recognition

Read these papers with focus on learning about the problem, how they model it and what kind of architecture they apply! Take note of any tweaks and tricks you find interesting but don't spend a lot of time trying to figure out all the details!

* Collobert et al. [Wav2Letter: an End-to-End ConvNet-based Speech Recognition System](https://arxiv.org/abs/1609.03193)
* Palaz et al. [End-to-end Phoneme Sequence Recognition using Convolutional Neural Networks](https://arxiv.org/abs/1312.2137)
* Baidu Research [Deep Speech 2: End-to-End Speech Recognition in English and Mandarin](https://arxiv.org/abs/1512.02595)
This paper is very dense. For now, only have a look at why and how they combine CNNs with RNNs in their model. FYI, [this paper](https://arxiv.org/abs/1412.5567) describes an earlier version.

### Visualization and Introspection

We will have a separate session on this topic but it won't hurt to have a look at this already.

* Zeiler & Fergus [Visualizing and Understanding Convolutional Networks](https://arxiv.org/abs/1311.2901)
* Yosinski et al. [Understanding Neural Networks Through Deep Visualization](http://yosinski.com/media/papers/Yosinski__2015__ICML_DL__Understanding_Neural_Networks_Through_Deep_Visualization__.pdf)
See also the [supplementary website and video](http://yosinski.com/deepvis). 

Optional: Maybe somebody would also like to have a look at the [Deep Visualization Toolbox code](https://github.com/yosinski/deep-visualization-toolbox). 

### More Optional Reading

There is a dedicated CNN thread in the [course forum](https://campusup.uni-potsdam.de/group/representation-learning/forum) where you can post links to interesting resources like papers, blogs or github repositories. As you explore the field, please post your findings, too! You can also link to your individual blog posts where you document what you found and learned. Use the "parking lot" thread in the forum to indicate advanced topics that we should look at later!

As a lot of the "RNN space" has remained largely uncharted, please feel free to also continue to further explore here as well.


## Auxiliary Demos

Andrej Karpathy has created very nice [CNN demos for MNIST and CIFAR-10 using ConvNetJS](http://cs.stanford.edu/people/karpathy/convnetjs/) that run directly in the web browser.


## Course Project: Getting to know the dataset

Please read the paper ["LibriSpeech: an ASR corpus based on public domain audio books"](http://www.danielpovey.com/files/2015_icassp_librispeech.pdf) which introduces the dataset used for the course project!


## The Practical Part: Building a CNN/RNN Recipes Collection

We continue with our efforts to build a recipes collection (cf. [last assignment](assignment2+3.html)) and extend the scope to CNN as well as combined approaches. 