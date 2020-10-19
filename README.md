# Deep_Learning_Recommender_System
I am going to explain how we integrate some deep learning models, in order to make an outfit recommendation system. We want to build an outfit recommendation system. You can train a neural network with user ratings or purchases, and use it to make recommendations; deep learning can be very good at recognizing patterns in a way similar to how our brain may do it. It's good at things like image recognition and predicting sequences of events.Neural networks are fundamentally matrix operations and there are already well-established matrix factorization techniques for recommender systems that fundamentally do something similar. In SVD for example, we find matrices that we multiply together using weights that are learned from stochastic gradient descent, it's almost the same thing, just thought of in a different way. So yeah, you could think of recommender systems as looking for patterns, just very complex ones based on the behavior of other people. So a matrix factorization can be modeled as a neural network. I think the main reason to experiment with applying neural networks to recommender systems is that it lets us take advantage of all the rapid advances in the fields of AI and deep learning. Amazon, for example, has open-sourced a system called DSSTNE, that's D-S-S-T-N-E, which allows you to run huge neural networks that deal with sparse data, on a cluster, efficiently. They claim to be using this internally for their own recommender systems. There are also ways to use TensorFlow in a cluster, and take advantage of a whole fleet of GPUs. And there's always research on new topologies for neural networks that can lead to fresh insights on how to make better recommendations using them. In some cases, approaches using neural networks have been shown to outperform SVD already, even if it's by a rather small margin. So, let's dive into some ways you can apply neural networks to the problem of making recommendations.
