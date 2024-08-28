# Bayesian Classification (Quadratic Multiclass Classification)
samples from three Gaussian distribution for each dataset described below:

**Dataset1:**

$$ class1:\quad\mu = \binom{3}{6} \qquad 
\sum =
\begin{pmatrix}
1.5 & 0 
\\
0 & 1.5
\end{pmatrix}
$$

$$ class2:\quad\mu = \binom{5}{4} \qquad 
\sum =
\begin{pmatrix}
2 & 0 \\
0 & 2
\end{pmatrix}
$$

$$ class3:\quad \mu = \binom{6}{6} \qquad 
\sum =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

**Dataset2:**

$$class1:\quad \mu = \binom{3}{6} \qquad 
\sum =
\begin{pmatrix}
1.5 & 0.1 \\
0.1 & 0.5
\end{pmatrix}
$$

$$class2:\quad \mu = \binom{5}{4} \qquad 
\sum =
\begin{pmatrix}
1 & -0.20 \\
-0.20 & 2
\end{pmatrix}
$$

$$class3:\quad \mu = \binom{6}{6} \qquad 
\sum =
\begin{pmatrix}
2 & -0.25 \\ 
-0.25 & 1.5
\end{pmatrix}$$


Consider the first 80% of the data in each class for train and the rest 20% for test and use a Bayesian classifier to classify both the train and test datasets.

### Dataset1 Plots
![alt text](https://github.com/Ghafarian-code/Bayesian-Classification-threeGaussianDistribution/blob/master/images/data1%204.jpg)
![alt text](https://github.com/Ghafarian-code/Bayesian-Classification-threeGaussianDistribution/blob/master/images/data1%203.jpg)
### Dataset2 Plots
![alt text](https://github.com/Ghafarian-code/Bayesian-Classification-threeGaussianDistribution/blob/master/images/data2%204.jpg)
![alt text](https://github.com/Ghafarian-code/Bayesian-Classification-threeGaussianDistribution/blob/master/images/data2%203.jpg)

### The main difference between two datasets
The datasets have the same mean but different covariances, which causes differences in their cross-sections. In Dataset 1, the covariance of each diagonal class and the areas on the main diameter are equal, so the cross-sections of the classes are circular, but because the covariance of each class is different from the others (values ​​on the main diameter), the size and elongation of the cross-sections of the classes are different. and as it is clear in the 3D palette, class two
It has more variance, it has more horizontal elongation, and class three, which has the lowest variance, is narrower and more elongated.
In Dataset 2, the covariances are not diagonal and the cross section of the classes are ovals with different sizes and in different directions (they are stronger in the feature direction).

### compare this part with bayasian-classification-oneGaussianDistribution?
In the second part of the previous exercise, we considered the covariance matrix of the classes to be the same, therefore, the cross section of the classes had the same shape and size and the decision boundary was linear, but in this exercise, due to the inequality of the covariances, the boundary separating the classes becomes non-linear.
