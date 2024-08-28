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
Both datasets have equal mean but different covariances, which causes the difference in their cross-section. 
In Dataset1, the covariance of each class is diagonal, and the elements on the main diagonal are equal, so the cross-sections of the classes are circular, but because the covariance of each class is different from the others (values ​​on the main diagonal ), the size and stretch of the cross-sections of the classes are different. As it is clear in the three-dimensional diagram, class2, which has more variance, has more horizontal stretch(positive kurtosis), and class3, which has the least variance, is narrower and more vertically stretched(negative kurtosis).
In Dataset2, the covariances are not diagonal and the cross-section of the classes are ovals with different sizes and in different directions(they are in the direction of stronger features).

### compare with Bayasian-classification-oneGaussianDistribution?
In Bayesian classification with one Gaussian distribution, we considered the covariance matrix of the classes to be the same, therefore, the cross-section of the classes had the same shape and size and the decision boundary was linear, but in this project, due to the inequality of the covariances, the boundary separating the classes becomes non-linear. 
