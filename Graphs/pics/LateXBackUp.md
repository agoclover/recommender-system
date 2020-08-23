欧氏距离

$$\begin{eqnarray}
d\left ( x,y \right ) & = & \sqrt{\sum_{i}^{ }\left ( x_i-y_i \right )^2  } 
\end{eqnarray}$$

余弦相似度

$$\begin{eqnarray}
cos\theta = \frac{a\cdot b}{||a||\times ||b||} 
\end{eqnarray}$$

基于 UGC 的推荐的最简单的算法

$$\begin{eqnarray}
p\left ( u, i \right ) =\sum_{b}^{} n_{u,b}n_{b,i}
\end{eqnarray}$$

TF-IDF

$$\begin{eqnarray}
TF-IDF = TF_{i,j} \times IDF_{i}=\frac{n_{i,j}}{n_{*,j}}\times log\frac{N +1}{N_{i}+1} 
\end{eqnarray}$$

TF-IDF 对基于 UGC 的推荐的改进

$$\begin{eqnarray}
p\left ( u, i \right ) =\sum_{b}^{} \frac{n_{u,b}}{log\left ( 1+n_{b}^{(u)}  \right ) } \frac{n_{b,i}}{log\left ( 1+n_{i}^{(u)}  \right )} 
\end{eqnarray}$$

矩阵因子分解

$$\begin{align}
R_{M\times N } & = P_{K\times M}^{T}\times Q_{K\times N}
\end{align}$$

损失函数

$$\begin{align}
C = \sum _{\left ( u,i \right ) \in R_{0}} \left ( R_{ui} - \bar{R}_{ui} \right ) ^2 + Reg = \sum _{\left ( u,i \right ) \in R_{0}} \left ( R_{ui} - P_u^T\cdot Q_i \right ) ^2 + \lambda \sum _{u}||P_{u}||^2 + \lambda \sum _{i}||Q_{i}||^2
\end{align}$$

