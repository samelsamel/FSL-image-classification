
# FSL? 

Few-Shot Learning is a sub-area of machine learning. It’s about classifying new data when you have only a few training samples with supervised information.

# Variations? 

1-N-Shot Learning (NSL)

2-Few-Shot Learning

3-One-Shot Learning (OSL)

4-Less than one or Zero-Shot Learning (ZSL)

**FSL means N-way-K-Shot-classification: N= nb of classes and K nb of samples.**

## Zero shot learning: 

The goal of Zero-Shot Learning is to classify unseen classes without any training examples.
You can do this is you have an idea about the object appearance, properties, and functionality


## One and few shot Learning:

Having one or more samples in the dataset. 

### N-way-K-Shot-classification approach 



A training (support) set that consists of:
* N class labels
* K labeled images for each class (a small amount, less than ten samples per class)
* Q query images

We want to classify Q query images among the N classes. The N * K samples in the training set are the only examples that we have.


The first and most obvious step in an FSL task is to gain experience from other, similar problems. 
This is why Few-Shot Learning is characterized as a **Meta-Learning problem**



In Meta-Learning, we learn how to learn to classify given a set of training data.


Two approaches: 


* Data-level approach (DLA)
* Parameter-level approach (PLA)



### Data-level approach

Basing on adding more data. 
The key feature of the base-dataset is that it doesn’t have classes that we have in our support-set for the Few-Shot task
This can be done using GAN's or data augmentation techniques. 


### Parameter-level approach

Problem: You can overfit on few samples 
That is why on the parameter-level we train our model to find the best route in the parameter space to give optimal prediction results. 
This technique is called Meta-Learning.


If you are interested in learning more about Meta Learning you can read more in here where this was taken from:
https://neptune.ai/blog/understanding-few-shot-learning-in-computer-vision

