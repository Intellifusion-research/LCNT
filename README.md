![image](https://github.com/Intellifusion-research/LCNT/blob/main/Figures/framework.png)

# LCNT

LCNT is a feature vector compression model for accelerating approximate nearest neighbor search. It can significantly recude the time cost of index construction and query latency without sacrificing search accuracy. This code in implemented in Pytorch 1.2.0. 

Code will be released soon.

Paper: [Learnable Compression Network with Transformer for Approximate Nearest Neighbor Search](https://arxiv.org/abs/2107.14415)

# Abstract

Approximate Nearest neighbor search (ANNS) plays a crucial role in information retrieval, which has a wide range of application scenarios. Therefore, during past several years, a
lot of fast ANNS approaches have been proposed. Among these approaches, graph-based methods are one of the most popular type, as they have shown attractive theoretical guarantees and low query latency. In this paper, we propose a learnable compression network with transformer (LCNT), which projects feature vectors from high dimensional space onto low dimensional space, while preserving neighbor relationship. The proposed model can be generalized to exiting graph-based methods to accelerate the process of building indexing graph and further reduce query latency. Specifically, the proposed LCNT contains two major parts, projection part and harmonizing part. In the projection part, input vectors are projected into a sequence of subspaces via multi channel sparse projection network. In the harmonizing part,a modified Transformer network is employed to harmonize features in subspaces and combine them to get a new feature. To evaluate the effectiveness of the proposed model, we conduct experiments on two million-scale databases, GIST1M and Deep1M. Experimental results show that the proposed model can improve the speed of building indexing graph to 2×-3× its original speed without sacrificing accuracy significantly. The query latency is reduced by a factor of 1.3 to 2.0. In addition, the proposed model can also be combined with other popular quantization methods.

# Experiments

![image](https://github.com/Intellifusion-research/LCNT/blob/main/Results/Table%201.png)

![image](https://github.com/Intellifusion-research/LCNT/blob/main/Results/Table%202.png)

![image](https://github.com/Intellifusion-research/LCNT/blob/main/Results/Table%203.png)





