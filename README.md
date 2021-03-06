# Keras/Apache Spark 
_*Team ARMS*_

## Overview

Through this assignment, we strive to introduce the basics of creating, training, and testing neural networks in Keras and well as utilizing the powers of Apache Spark. We start off by providing simple problems with lots of prewritten code to exemplify how various Keras functions and classes while probing the student to somewhat conceptually understand them. After this, we move on to more free flow tasks like implementing high-performing models from scratch or debugging existing code to really test and grow the students ability to apply the concepts they have learned.

## How to Navigate this Repository

The assignment is located under the 'Homework' directory while the notes and slide deck can be found under 'Documentation'. Obviously, the homework requires moderate levels of comprehension of the notes and slides to begin. Within the homework directory, there are two directories, 'Problems' which contains the problems/tasks that are given to the student and 'Solutions' which contains possible answers to the coding and conceptual questions. The order in which we expect students to complete this is as following (with intended time written adjacently):

* 'Problem 1 - Pythagorean Distance' (45 minutes)
* 'Problem 2 - MNIST Classification Walkthrough' (1.5 hour)
* 'Task 1' (1.5 hour)
* 'Task 2' (45 minutes)

The naming is such that the "problems" are far more guided with more skeleton code while "tasks" are more freeform with a few hints of what to try. The solutions for the tasks, especially task 1, are just one in many that work. As long as the student achieves the desired level of accuracy, any implementation is acceptable. 

Finally, the quiz to check comprehension is located under the 'Quiz' directory. 

## Objective 1: Introduction to Keras

By far the most common use of Keras is to create sequential models, the simplest of which is the multi-layer perceptron (MLP). Unfortunately, there are quite a few aspects of Keras that must be understood before being able to implement your own MLP. The lecture covers all of these (initiating a sequential model, creating an input layer, adding hidden layers, and so on), however, its one thing to see it in lecture and another to be able to interact with the code. That is the goal of 'Problem 1 - Pythagorean Distance.' Without modification, it contains the full code to create training data for the pythagorean distance problem, feed it into a neural network (albiet not a very good one), and test the results. The questions in this assignment are largely conceptual and have the students play around with parameters of the model to see how they affect performance. Additionally, the last question serves as a "hype-deflating" one, questioning whether neural networks are effective, especially with a problem as simple as this one.

## Objective 2: Image Classification

After somewhat showing that neural network regression works, we try to apply Keras to a more relevant process. Especially in the last decade, one of the flagship applications of ML has been to classify images. The MNIST dataset, a collection of handwritten digits 0-9, is our selection of what to explore for this application because it's a problem thats relatively easy to solve, doesn't require a whole lot of preprocessing, and has fairly low dimensionality. The exploration starts in 'Problem 2 - MNIST Classification Walkthrough.' We begin by exploring the data a little bit: since this is, in fact, an image problem, the first step is to visualize the inputs to get a sense for what they look like. After that, we want to do some basic preprocessing to make sure our neural network will work effectively. We then start testing how well students have understood the concepts from the previous problem by asking them to implement an MLP for MNIST classification (which doesn't perform too great, but also doesn't do terrible). Since the "flatten" layer is new, that is provided in the skeleton code. Now, since the student understands the challenge at hand and is motivated to find a better solution, we introduce the idea of convolutional neural networks. These are fairly involved in syntax so a lot of the code is provided. Finally, data generators are introduced but not explored in much detail.

With all this knowledge at hand, we then transition to a much more hands on exercise, 'Task 1.' In this one, we provide various hints for how to improve the accuracy of the model, but then let the student free to explore their own ideas. Here, we also link to the Keras documentation so that they get a sense of what its like to read about and implement new features from any ML libraries they might encounter online. Although the task is fairly difficult, completing is should feel very eye-opening and rewarding.


## Objective 3: Debugging Keras Models

Especially when working in large-scale projects, the skill of being able to look through models and get a sense of how they work and how to improve them is crucial. Therefore, to wrap up Keras, in 'Task 2' we provide a pre-implemented model for a fairly basic input/output relationship which seems to not perform particularly well. The student, using all the information gained in the previous parts about the strengths/weaknesses of neural networks, can experiment around with the code until they find out how to tweak it to signficantly improve its accuracy. Its intentional that the generated dataset is fairly large to make sure the student is reserved in how many changes they attempt: in projects with terabytes of training data, experimentation must be smart to assure time is not wasted. 

