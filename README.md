# Support Vector Machine

## Definition

Support Vector Machines (SVM) algorithm is used to find a separating line/hyperplane between data of different classes. SVM works by maximizing the distance to the nearest point of each classes, which we call a margin.
SVM is a <strong>Supervised Learning</strong> algorithm. 

<img src="https://miro.medium.com/max/1088/1*6U9NrruycDBsPOyivpn8UQ.png" width="400">

## Parameters of SVM: Kernels, C, Gamma

* Kernels: creates different shapes of decision boundary. Some kernels types are linear, rbf, polynomial, and sigmoid.
* C: controls tradeoff between smooth decision boundary and classifying training points correctly (accuracy). Higher C -> more complex -> risk overfit (high variance). Lower C-> simpler -> risk underfit (high bias).
* Gamma: defines how far the influence of training examples in creating the decision boundary. Low  values -> far reach, means data far from the boundary is included in the calculation of decision boundary. High values -> close reach, means only the data near the boundary are involved in calculating the decision boundary.

Kernels, C, and Gamma determines the model fit (underfit, overfit, good fit). 

## Advantages 

* Effective in high dimensional spaces where there are ckear margins of separation.
* Still effective in cases where number of dimensions is greater than the number of samples.
* Uses a subset of training points in the decision function (called support vectors), so it is also memory efficient.
* Versatile: different Kernel functions can be specified for the decision function. Common kernels are provided, but it is also possible to specify custom kernels.

## Disadvantages 

* Doesn't perform well in very large datasets: high training time, slow.
* Doesn't work well with lots and lots of noise, prone to overfit with the noise.
* If the number of features is much greater than the number of samples, avoid over-fitting in choosing Kernel functions and regularization term is crucial.
* SVMs do not directly provide probability estimates, these are calculated using an expensive five-fold cross-validation

## References

https://www.youtube.com/watch?v=I74ymkoNTnw
https://scikit-learn.org/stable/modules/svm.html
