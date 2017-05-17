# Backprogagation Algorithm

### 简介

多层感知器网络（MLP），至少包含一个隐层（Hidden Layer）。多层感知器网络的计算，甚至不会比单层感知器网络复杂。这要归功于巧妙利用矩阵、向量计算。需要提供初始权值，再迭代求权值参数。主要使用算法是 Backpropagation Alogrithm。

- 刷新，由输出层到输入层反向刷新
- MLP，multilayer perceptron

### 组成

- Input Layer

- Hidden Layer

- Output Layer

- Weights

- Activation Function: 
  $$
  Sigmoid Function:      f(net_1)=\frac{1}{1+e^{-net_i}}
  $$


### 网络函数

每一个神经元都有自己的网络函数，记为
$$
net_l=\sum_{k=1}^nw_{lk}x_k ，(1\leq l\leq m)
$$
n，为输入向量的分量个数

m，为人工神经元个数



