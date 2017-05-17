# Adaline Network

### 简介

和 perceptron network 不同，Adaline 不需要迭代。无需提供初始权值。通过解正规方程组来得到解。



### 网络函数

$$
y=\sum^n_{i=0}w_ix_i
$$

### 激活函数

$$
z=\varphi(y)
$$



### 特征

- 两类线性可分
- 单层感知器网络
- 向前网络
- 多输入，单输出


$$
E=\frac{1}{2}\Vert T-XW \Vert^2_2
$$


### 实例

- 正例

  - AND

    ```
    x        o

    x        x
    ```

  - OR

    ```
    o        o

    x        o
    ```


- 反例

  - XOR，线性不可分

    ```
    X        o

    o        x
    ```

    ​

  ​