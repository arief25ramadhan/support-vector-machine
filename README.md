# Support Vector Machine

## Definition

Support Vector Machines (SVM) algorithm is used to find a separating line/hyperplane between data of different classes. SVM works by maximizing the distance to the nearest point of each classes, which we call a margin.
SVM is a <strong>Supervised Learning</strong> algorithm. 

<img src="https://miro.medium.com/max/1088/1*6U9NrruycDBsPOyivpn8UQ.png" width="400">

## Advantages 

* Effective in high dimensional spaces.
* Still effective in cases where number of dimensions is greater than the number of samples.
* Uses a subset of training points in the decision function (called support vectors), so it is also memory efficient.
* Versatile: different Kernel functions can be specified for the decision function. Common kernels are provided, but it is also possible to specify custom kernels.

## Disadvantages 

* If the number of features is much greater than the number of samples, avoid over-fitting in choosing Kernel functions and regularization term is crucial.
* SVMs do not directly provide probability estimates, these are calculated using an expensive five-fold cross-validation

## References

https://www.youtube.com/watch?v=I74ymkoNTnw
https://scikit-learn.org/stable/modules/svm.html
