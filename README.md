# 3D Model Recognition based on two layers Few-Shot Learning Network

Implementation of the paper:  <a href="/pdf/draft.pdf">3D Model Recognition based on two layers Few-Shot Learning Network</a>. The code is coming.

## 1. Abstract
With the development of multimedia technology, 3D model has been applied in many fields such as mechanical design, construction industry, entertainment industry, medical treatment and so on. The number of 3D model is becoming more and more in our lives. Therefore, effective automatic management and classification of 3D models become more and more important. In this paper, we propose a dual-meta-learner model based on LSTM to learn the exact optimization algorithm used to train another two learner neural network classifier in the few-shot regime. The parametrization of our model allows it to learn appropriate parameter updates specifically for the scenario where a set amount of updates will be made, while it can also achieve a general initialization of the learner (classifier) network that allows for quick convergence of training. Our method attains state-of-the-art performance by significant margins.

## 2. Contributions
- We propose a novel dual-meta-learner model based on two-layer LSTM that uses a small amount of 3d model data to generalize to a large amount of unlabeled 3D model data.
- By generalizing the training on small databases to large databases, the classification effect is comparable to the latest method, but we use less computational cost and time cost.

## 3. Databases

in our approach, we converted the multiple datasets into a whole called meta-sets **D**, and divided each dataset into the training set and the test set. The organization of dataset is shown as Figure.1.

![](/pic/figure1.png)

## 4. Approach
Here we present a method to solve the weakness of a neutral network trained by a gradient based optimization for a few shooting learning problems by constructing problems in a meta-learning environment. We propose an LSTM based dual meta-learner optimizer that is trained to optimize the learner neural network classifier. Meta-learners capture short-term knowledge in tasks and long-term knowledge common to all tasks. The meta-learners model is trained to quickly aggregate learner classifiers into good resolutions on each task by using the goal of direct capture optimization algorithms with the ability to have good generalization performance given only a certain number of updates. In addition, the development of our meta-learner model allows it to learn the tasks of the learner classifier to co-initialize, which captures the basic knowledge shared between all tasks. We want to generalize a small amount of labeled 3D model data to a large number of unlabeled 3D model data, and then test the classification.

![](/pic/figure2.png)

## 5. Authors
- Jie Nie
- Xu Ning 
- Ming Zhou
- Ge Yan
- Zhiqiang Wei

## 6. Acknowledgement
The code is available **soon**.

