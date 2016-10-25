---
layout: default
title: Assignment 2 & 3
id: ass2
---


# Assignments 2 & 3: RNN Exploration

In these assignments, we will jump right the realm of some of the most successful neural network designs: recurrent and recursive neural networks.

If you have not completed [assignment 1](assignment1.html) yet, make sure to catch up and finish all tasks before you continue!

As October 31 is a public holiday, there will be no class. Hence, you will have 2 weeks for these assignments and to prepare for the next class on November 7. I strongly advice to start working on the assignments right away.

I further recommend teaming up (loosely) and using the "wisdom of the crowd" wherever necessary. Helping each other is encouraged and will not be considered "cheating." Remember: The assignments are *not* meant for grading or to keep you busy. You are supposed to learn something and gain hands-on experience. This can be a lot of fun in a group. If you are looking for people to team up with, just use the [course forum](https://campusup.uni-potsdam.de/group/representation-learning/forum).


## Basic Reading

Please start by reading the full [Deep Learning Book - Chapter 10: Sequence Modeling: Recurrent and Recursive Nets](http://www.deeplearningbook.org/contents/rnn.html). This should give you a good overview of this domain and forms a common basis for everybody.

Post your remarks, insights and open questions in your blog and in the forum! Help each other to make sure you are not getting stuck too long with some unresolved issue.

Deadline for questions to be considered in class is *November 5, 7am*. 
I will also try to accommodate things that come in later but I cannot make guarantees. The earlier you bring up questions, the better.

## Explore!

Of course - as with all quickly evolving fields like deep learning - the book chapter only covers the "tip of the iceberg." There is much more exciting stuff to explore. And I would like us all to go out and find it. 

This is a crowd effort. It is totally impracticable that everybody reads everything. Everybody has slightly different interestes anyway. Investigate what you find interesting and share it with the others!

As a starting point, I will open a dedicated RNN thread in the [course forum](https://campusup.uni-potsdam.de/group/representation-learning/forum) and post links to interesting resources like papers, blogs or github repositories. As you explore the field, please post your findings, too! You can also link to your individual blog posts where you document what you found and learned. 

In class on November 7, we will bring all the bits and pieces together and create a "big picture."

You might come across things that look too advanced at the current stage, but it might be interesting to explore them later in the course. I have opened a dedicated "parking lot" thread in the [course forum](https://campusup.uni-potsdam.de/group/representation-learning/forum) for this. Please feel free to add suggestions! Remember, roughly the second half of the course is so far largely unplanned. So there is plenty of space where we could cover such topics.



## The Practical Part: Building an RNN Recipes Collection

You will likely find that the basic theory behind RNNs is less complicated than expected. It is oftentimes quite straightforward to draw up an RNN model for a specific learning task. However, it is less straightforward to implement the concept within a specifc software framework and then successfully train it.

Before we set out to design and train RNNs ourselves, we are therefore going to first figure out how others have done it. Again, this is a collaborative effort. Everybody picks what they are interested in. We would like to get broad coverage of the standard architectures covered in the book chapter and beyond - with implementations in the different software frameworks and applications to various problem domains.

Here is what needs to be done specifically:

* Whenever you come across an RNN implementation (preferably related to a paper) that is based on Theano or Tensorflow (in pure low-level code or using frameworks like Keras or Blocks) post a link in the forum - but please avoid duplicates!
* If it is code to build and train the model, try to run it for a few epochs to get an idea of the training performace! (No need to fully train it! We are interested in implementation recipes.)
Plot the computation graph and compare it with what you would expect from the description / code! Are any interesting tweaks, hacks or extensions used?
* If trained model parameters are provided, look at ways to visualize them! (No need to write tons of custom code yet! We want to find out how much we can already do with available tools.) Run the model (without training) on some test data if available.

Whenever you are doing something like this, leave a note in the forum to let the others know (for "load balancing") and report your experiences in a short blog post afterwards.
Together, we should be able to create quite a collection of working examples and get an idea what we like and dislike about the different software frameworks.