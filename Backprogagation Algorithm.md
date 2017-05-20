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




### 激活函数

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



### BP 算法推导


$$
\frac {\partial E} {\partial net^{(2)}}=F^{'(2)}(net^{(2)})W^{(3)^T}S^{(3)} =
\left[ \begin{array}{ccc}
     f^{'(2)}(net_1^{(2)}) & 0 & 0 \\  0 &f^{'(2)}(net_2^{(2)})& 0  \\  0 &  0 & f^{'(2)}(net_3^{(2)}) \end{array} \right]
\left[ \begin{array}{cc}
     w_{11}^{(3)} & w_{21}^{(3)}  \\ w_{12}^{(3)} & w_{22}^{(3)}  \\ w_{13}^{(3)} & w_{23}^{(3)} \end{array} \right]
\left[ \begin{array}{c}
    - \frac {\partial E}{\partial net_1^{(3)}} \\ - \frac {\partial E}{\partial net_2^{(3)}} \\ \end{array} \right]
$$


### 刷新过程

相当于寻找梯度为0，的更新迭代过程



### 应用

- MPL 主要应用于数据分类
- 函数逼近



> Note:多层感知器网络，所有激活函数都为线性，那么这个 MPL 可以等价于一个单层感知器网络