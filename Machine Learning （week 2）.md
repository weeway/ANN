# Machine Learning （week 2）

### Gradinet Decent

#### 学习率 alpha

- 学习率太大会导致代价函数的值，随迭代次数，不降反升
- 学习率不刚好还可能导致代价函数的值，随迭代次数，呈先增后减的趋势
- 学习率太小又可能导致，收敛所需的迭代次数增多



#### 梯度下降（theta 学习）

$$
Θ_{new}=Θ-A^T(AΘ-y)
$$


$$
\begin{bmatrix}
    x_{11} & x_{21} & x_{31}  \\
    x_{12} & x_{22} & x_{32}  \\
    x_{13} & x_{23} & x_{33}  \\
    x_{14} & x_{24} & x_{34}
\end{bmatrix}
\Bigg(
\begin{bmatrix}
    x_{11}       & x_{12} & x_{13} & x_{14} \\
    x_{21}       & x_{22} & x_{23} & x_{24} \\
    x_{31}       & x_{32} & x_{33} & x_{34}
\end{bmatrix}
\begin{bmatrix}
    Θ_{1} \\ Θ_{2} \\ Θ_{3} \\ Θ_{4} 
\end{bmatrix}
-
\begin{bmatrix}
    y_{1} \\ y_{2} \\ y_{3}
\end{bmatrix}
\Bigg)
$$


### Normal Equation

$$
\mathbf{A} x = b \\
\mathbf{A}^T\mathbf{A}x=\mathbf{A}^Tb \\
x=(\mathbf{A}^T\mathbf{A})^{-1}\mathbf{A}^Tb
$$

ATA 不可逆的话，可能会有以下的问题：

- 特征冗余，如特征间线性相关（eg. a=pow(x,2),b=pow(x,3)）
- 特征太多，导致特征数大于样例数





