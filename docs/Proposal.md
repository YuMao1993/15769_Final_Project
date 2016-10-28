### 15769 - Visual Computing System Final Project
 How to effectively **scale up** and **scale out** the candidate binary feature matching algorithms? In this project, we will optimize and parallelize **LSH** and **Hierarchical Clustering** on both CPU and GPU. We will also design specific strategies to scale them out on a cluster of nodes. 
 Our library will only be focusing on ANN search within Hamming space. With this knowledge, how can we improve the algorithm auto-selection part in [FLANN](http://www.cs.ubc.ca/research/flann/).
 The algorithm auto-selection strategy proposed in [3] requires evaluating at least on one tenth of the dataset. How to effectively parallelize and scaling out the auto-selection algorithm on a cluster of nodes?
 **Data set**: For optimization and parallelization on single machines we will be working on small dataset like CIFAR-10 and Caltech256. For scaling out the framework, we will be working on large dataset like ImageNet.
 **Machine**: a cluster of GPU nodes
 **Code**: We will be referencing [FLANN](http://www.cs.ubc.ca/research/flann/) to gain a better understanding of [3]. We will probably reuse/integrate some FLANN code into our framework.
 week 1: Read [1][2][3].
 week 2: Set up FLANN and get familiar with the code.
 week 3~4: Implement and optimize **LSH** and **Hierarchical Clustering** on both CPUs and GPUs.
 week 5: Design and implement a better strategy for automatic algorithm selection specifically for binary features.
 week 6: Scale out LSH, Hierarchical Clustering and automatic algorithm selection onto a cluster.
 Optional: Build an example CBIR system based on our framework by deploying a imaging hashing stage with the deep learning approach proposed by [4]